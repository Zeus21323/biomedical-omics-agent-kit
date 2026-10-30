# 通用 stdio 接入

任何支持 MCP 的客户端都按下面两条信息配置即可：

| 项 | 值 |
|---|---|
| 传输 | stdio（一行一条 JSON-RPC 2.0） |
| 命令 | `python` |
| 参数 | `<本仓库绝对路径>/mcp/biomedical_mcp.py` |
| 环境变量 | 无 |
| 依赖 | Python 3.9+，仅标准库 |

## 客户端侧要做的事

1. 以子进程方式拉起上面的命令，保持 stdin/stdout 连接；
2. 发送 `initialize`（`protocolVersion: 2024-11-05`）；
3. 收到 `initialize` 响应后，后续按 MCP 规范调用 `tools/list` 与 `tools/call`；
4. 不要向 stdout 打日志——stdout 是协议通道，日志请走 stderr。

## 自检

```bash
printf '%s\n' '{"jsonrpc":"2.0","id":1,"method":"initialize","params":{"protocolVersion":"2024-11-05","capabilities":{},"clientInfo":{"name":"t","version":"1"}}}' | python mcp/biomedical_mcp.py
```

应立刻返回一条 `initialize` 响应，其中 `serverInfo.name` 为 `biomedical-data`。
