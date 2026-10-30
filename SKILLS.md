# 技能索引

224 个技能，分 10 个主题。每个技能是一个目录，读取其中的 `SKILL.md` 即可获得完整说明。

## 转录组上游与定量（32）

| 技能 | 说明 |
|---|---|
| `nfcore-drop` | 当患者 RNA 数据及适配参考队列需要寻找异常表达或剪接时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/drop。 |
| `nfcore-isoseq` | 当已有 PacBio 全长 RNA 数据，希望整理转录本或辅助基因组注释时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/isoseq。 |
| `bulk-rnaseq` | End-to-end bulk RNA-seq orchestrator — takes raw FASTQ reads through QC and trimming (FastQC, fastp/Trim Galore), alignment and quantification (STAR, Salmon, featureCounts), assembles a gene-level cou… |
| `04-transcriptomics-5-utr` | 用于分析UTR、Kozak、IRES、uORF、poly(A)位点、密码子偏好和tRNA适配等转录后与翻译调控元件。 |
| `04-transcriptomics-alternative-splicing` | 当用户问表达没变是否剪接变了、同一基因在不同细胞为何不同、长短读长结果矛盾，或需剪接和异构体状态证据整合（IsoformStateDB方向）时使用；先查读段、覆盖和注释，不要求用户选择算法或懂PSI。 |
| `04-transcriptomics-fusion-transcript-detection` | 用于从RNA-seq检测基因融合或嵌合转录本，整理断点、分裂读段、跨越读段、阅读框和假阳性证据。 |
| `04-transcriptomics-m6a` | 用于分析m6A、m5C等RNA修饰的富集区或候选位点；支持抗体富集、化学转换、交联和Nanopore直接RNA等不同证据。 |
| `04-transcriptomics-mirna-analysis` | 用于按文库类型分析miRNA、lncRNA或circRNA的表达、注释、差异和候选调控关系。 |
| `04-transcriptomics-rbp-regulation` | 用于从eCLIP、iCLIP及其他CLIP-seq协议定位RNA结合蛋白位点，并评估交联事件、背景、基序和重复一致性。 |
| `04-transcriptomics-ribo-seq` | 用于从Ribo-seq读段校准P-site、评估三核苷酸周期性、识别翻译ORF，并与匹配RNA-seq联合估计翻译效率。 |
| `04-transcriptomics-rna-editing` | 用于从RNA-seq识别A-to-I等RNA编辑候选，并排除胚系或体细胞DNA变异、链方向错误和比对伪影。 |
| `04-transcriptomics-rna-quantification` | 当用户已有bulk RNA-seq测序文件、FASTQ或比对结果，想得到各样本基因表达量或后续分析用的矩阵，或遇到链特异性、片段偏倚、基因编号和参考注释不一致时使用；已有可用矩阵则转入适当下游，不重复定量。 |
| `04-transcriptomics-transcript-assembly` | 用于从短读RNA-seq或长读RNA数据重建转录本、发现异构体、合并样本注释并控制组装膨胀。 |
| `nfcore-alleleexpression` | 当RNA 数据及匹配基因型可用于研究等位基因表达不平衡时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/alleleexpression。 |
| `nfcore-cageseq` | 当转录起始相关 CAGE 测序需要提取标签和起始位点时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/cageseq。 |
| `nfcore-circrna` | 当RNA 测序需要识别环状 RNA 或比较反向剪接信号时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/circrna。 |
| `nfcore-clipseq` | 当RNA 蛋白结合实验的 CLIP、iCLIP 或 eCLIP 数据需要处理时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/clipseq。 |
| `nfcore-dartseq` | 当带编辑标记的 RNA 数据需要分析修饰相关位点时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/dartseq。 |
| `nfcore-denovotranscript` | 当没有合适参考基因组，已有双端 RNA 测序并希望重建转录本时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/denovotranscript。 |
| `nfcore-dualrnaseq` | 当共测定 RNA 数据来自宿主与病原，需要分别定量或研究感染反应时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/dualrnaseq。 |
| `nfcore-lncpipe` | 当RNA 数据需要发现或整理长非编码 RNA 候选时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/lncpipe。 |
| `nfcore-nanostring` | 当已有 nCounter 计数、探针 panel 或 RCC 交付数据，需要表达比较时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/nanostring。 |
| `nfcore-nascent` | 当新生转录实验的 PRO、GRO 或 NET 类测序需要信号分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/nascent。 |
| `nfcore-riboseq` | 当核糖体足迹测序需要定位翻译区域或估计翻译效率时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/riboseq。 |
| `nfcore-rnafusion` | 当RNA 测序需要寻找融合转录本或复核融合候选时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/rnafusion。 |
| `nfcore-rnaseq` | 当测序报告或建库证据表明是普通整体 RNA 测序，需要整理表达或比较样本时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/rnaseq。 |
| `nfcore-rnasplice` | 当RNA 测序及样本分组用于研究可变剪接或转录本使用变化时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/rnasplice。 |
| `nfcore-rnastructurome` | 当DMS 或 SHAPE 等 RNA 化学探测数据需要反应性或结构相关分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/rnastructurome。 |
| `nfcore-slamseq` | 当代谢标记 SLAM-seq 数据需要估计新生 RNA 比例或动力学时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/slamseq。 |
| `nfcore-smrnaseq` | 当小 RNA 建库数据需要识别 miRNA 或其他短 RNA 并定量时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/smrnaseq。 |
| `nfcore-stableexpression` | 当多个表达数据集需要筛选在指定条件下稳定的参考基因时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/stableexpression。 |
| `rna-modification-clip` | \| Peak analysis for RNA modification and RNA-protein interaction sequencing: MeRIP-seq/m6A (exomePeak2 peak calling and differential methylation), RIP-seq (general peak calling with input control) and… |

## 差异表达与功能富集（11）

| 技能 | 说明 |
|---|---|
| `gwas-functional-interpretation` | 当用户有疾病遗传关联结果，不知道涉及什么通路、组织或细胞类型、想补机制解释和富集图，或提出MAGMA/分层LDSC时使用；区分遗传信号富集与普通基因列表富集。 |
| `04-transcriptomics-b05-t03` | 用于全量排序特征的GSEA以及GSVA、ssGSEA样本级基因集评分；当用户需要通路方向、leading-edge基因或每个样本的通路分数时使用。 |
| `pathway-enrichment` | Run pathway and gene-set enrichment analysis on gene lists or ranked gene data, then interpret the results. Use whenever the user has a set of genes (differentially expressed genes from PyDESeq2/Scanp… |
| `pathway-enrichment-analysis` | 用于基因、蛋白或代谢物列表的GO、KEGG、Reactome等过度富集分析；当用户已有候选特征集合和明确背景集时使用。 |
| `pydeseq2` | Differential gene expression analysis for bulk RNA-seq with PyDESeq2, including formulaic designs, Wald tests, FDR correction, LFC shrinkage, and result visualization. |
| `04-transcriptomics-deseq2` | 当用户已有bulk RNA-seq基因计数或差异分析结果，想知道两组哪些基因不同、制作差异基因热图，或遇到低表达、批次、配对、重复测量和结果冲突时使用；核查数据与设计后选择DESeq2、edgeR或limma-voom，已有结果从对应阶段继续，不因美化图件重跑检验。 |
| `metabolomics-differential-multivariate-stats` | 当用户需要对质控后的代谢矩阵进行样本级差异、PCA 和监督建模，并用正确验证识别批次驱动或过拟合结果时使用。 |
| `microbiome-differential-abundance` | 用于微生物特征表的组成型差异丰度建模、协变量校正和结果解释；当用户询问哪些菌或通路在组间变化时使用。 |
| `nfcore-differentialabundance` | 当已有表达或特征矩阵和样本背景，希望比较处理条件时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/differentialabundance。 |
| `pathway-enrichment-scaffold-replace` | 当用户需要把带证据等级的代谢物及效应映射到物种匹配的通路，并控制 ID 歧义、检测背景和重复特征造成的偏倚时使用。 |
| `single-cell-differential-abundance` | 当用户需要比较条件间离散细胞群或连续邻域的丰度变化，以供体为重复并处理组成数据的相互依赖时使用。 |

## 单细胞基础分析（20）

| 技能 | 说明 |
|---|---|
| `scanpy` | Standard single-cell RNA-seq analysis pipeline. For quality control (QC), normalization, dimensionality reduction (PCA/UMAP/t-SNE), clustering, differential expression analysis, and visualization. Bes… |
| `05-single-cell-virtual-cell-b01-t01` | 当用户拿到单细胞表达文件不知道质量是否可用，想清理低质量细胞、查看过滤前后变化，或发现QC图空白、质量指标缺失、过滤后细胞骤减时使用；涵盖10x及其他scRNA-seq计数数据的预处理与质量控制。已有对象先核查当前阶段，不要求用户知道列名、计数层或质控软件。 |
| `05-single-cell-virtual-cell-b01-t02` | 当用户需要把 scATAC-seq FASTQ 或 fragments 转成经过条形码、片段质量和可及性检查的 tile/peak 矩阵时使用。 |
| `05-single-cell-virtual-cell-b01-t03` | 当用户需要处理 10x Multiome 等同细胞多模态数据，保持条形码配对，分别质控各模态后再建立联合表示时使用。 |
| `05-single-cell-virtual-cell-b01-t04` | 当用户需要整合多样本、平台或队列的单细胞数据，在减少技术差异的同时检测过校正和真实条件信号丢失时使用。 |
| `05-single-cell-virtual-cell-b02-t01` | 当用户需要按样本识别液滴单细胞数据中的异型和同型双细胞，并区分技术混合与真实过渡或活化状态时使用。 |
| `05-single-cell-virtual-cell-b02-t02` | 当用户需要估计 droplet scRNA-seq 空液滴中的环境 RNA，并在保留原始计数的前提下校正受污染细胞时使用。 |
| `05-single-cell-virtual-cell-b02-t03` | 当用户发现单细胞线粒体比例很高、全为零或缺失，想判断细胞质量、解释线粒体比例图，或担心过滤删掉真实细胞群时使用；结合组织、物种、基因标识和其他质量指标核验计算与过滤规则，不要求用户选择统一百分比阈值。 |
| `05-single-cell-virtual-cell-b03-t01` | 当用户想把单细胞分成可靠群体、不知道该保留多少维或分多少群，已有PCA图看不懂、标签挤在一起，或UMAP结果不稳定时使用；涵盖PCA/LSI、邻居图与聚类，先检查质控对象和已有结果，不要求用户知道算法、软件或技术参数。 |
| `05-single-cell-virtual-cell-b04-t04` | 当用户问这些细胞是什么、细胞名字是否正确、两种注释结果冲突、疾病细胞是否被误标，或需要细胞注释、参考映射、scDiagnostics诊断时使用；从对象、marker和参考主动识别注释及复核需要，保留未知、新状态和低置信标签。 |
| `nfcore-hadge` | 当单细胞混样数据需要借助基因型或样本标签恢复供者身份时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/hadge。 |
| `nfcore-marsseq` | 当已确认板式 MARS-seq 数据，需要按孔位和分子标签整理表达时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/marsseq。 |
| `nfcore-scdownstream` | 当收到单细胞表达矩阵、H5AD 或分析对象，需要细胞质控、注释与组间研究时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/scdownstream。 |
| `nfcore-scflow` | 当已有历史单细胞表达对象，需要评估归档分析路径或复现处理时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/scflow。 |
| `nfcore-scnanoseq` | 当单细胞长读 RNA 数据需要恢复细胞身份并分析转录本时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/scnanoseq。 |
| `nfcore-scrnaseq` | 当建库或交付证据表明是单细胞 RNA 原始读段，需要生成细胞表达矩阵时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/scrnaseq。 |
| `nfcore-smartseq2` | 当已确认板式 Smart-seq2 测序，需要按细胞或孔位整理表达时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/smartseq2。 |
| `single-cell-format-io` | 当用户需要在 h5ad、Seurat、loom、10x HDF5/MTX 等格式间转换单细胞对象，并验证矩阵层、元数据和稀疏结构没有静默丢失时使用。 |
| `single-cell-staged-workflow` | 当用户收到单细胞测序文件不知道从何开始、希望把数据分析成课题结果、需要从已有AnnData继续或恢复失败流程，或指定EISCA时使用；根据实际文件、建库和已完成阶段安排可复现的分阶段工作流，不要求用户认识Nextflow或选择工具。 |
| `sc-rna-seq-analysis` | \| Single-cell RNA-seq comprehensive analysis pipeline. Covers 17+ analysis modules: QC, decontX, doublet detection, normalization, PCA, Harmony, clustering, UMAP (2D/3D), cell type annotation (SingleR… |

## 单细胞高级与虚拟细胞（20）

| 技能 | 说明 |
|---|---|
| `scgpt` | 使用单细胞生物学基础模型 scGPT 对单细胞表达数据进行嵌入和注释。适用于：从 AnnData 生成细胞嵌入以进行聚类或整合；执行零样本或微调后的细胞类型注释；为扰动或基因调控网络任务生成基因级表示。对于 scVI 等概率单细胞模型，请使用 scvi-tools 库。 |
| `scvi-tools` | 使用 scvi-tools 对单细胞 RNA 测序数据进行概率建模——使用 scVI 获得批次校正的潜在空间，使用 scANVI 进行半监督标签转移，并执行贝叶斯差异表达分析。适用于整合多个 scRNA-seq 批次、生成细胞嵌入以进行聚类、将参考数据的注释转移到查询数据，或按细胞簇评估差异表达基因。空间解卷积或映射应改用 cell2location、DestVI 或 Tangram。 |
| `05-single-cell-virtual-cell-b05-t02` | 当用户需要为细胞周期、应激、干扰素、耗竭等连续程序评分，并区分状态变化与细胞类型组成变化时使用。 |
| `05-single-cell-virtual-cell-b06-t03` | 当用户需要使用剪接动力学估计细胞状态变化方向，并结合转移模型评估潜在起始、终末状态和命运概率时使用。 |
| `05-single-cell-virtual-cell-b06-t05` | 当用户需要在有生物学连通依据的细胞谱系内重建分支和伪时间，并检验根节点、批次和供体对轨迹的影响时使用。 |
| `05-single-cell-virtual-cell-b08-t04` | 当用户问哪些细胞在互相影响、某基因是否参与细胞间传话、疾病或治疗前后通讯有何变化，或已有单细胞/细胞通讯结果却只有矩阵、缺网络弦图、图太乱或不同数据总出现相同分子时使用；涵盖配体–受体推断、条件比较、结果复用和适用图集。只有疾病、发表或毕业愿望时先识别问题与数据，不直接运行。 |
| `05-single-cell-virtual-cell-b09-t01` | 当用户需要分析 CRISPR Perturb-seq、CRISPRi/a 数据，将 guide 可靠分配到细胞并估计扰动的平均效应和状态依赖效应时使用。 |
| `05-single-cell-virtual-cell-b09-t04` | 当用户需要使用已训练单细胞模型预测基因敲除、过表达或其他扰动后的表达状态，并评估训练域和校准限制时使用。 |
| `05-single-cell-virtual-cell-b09-t05` | 当用户需要利用单细胞基线和扰动图谱预测药物在不同细胞状态中的响应，并明确剂量、时间和训练域外推风险时使用。 |
| `05-single-cell-virtual-cell-b10-t01` | 当用户需要联合分析 CITE-seq 的 RNA 与抗体衍生标签，校正 ADT 背景并为每个细胞选择合理的模态权重时使用。 |
| `05-single-cell-virtual-cell-b10-t03` | 当用户需要联合分析同一单细胞的基因组DNA与转录组数据，并关联变异、拷贝数、等位基因和表达状态时使用。 |
| `metabolite-mediated-cell-communication` | 当用户问细胞释放的代谢物是否影响其他细胞、某代谢物或转运体与疾病微环境有什么关系，或已有MEBOCOST/代谢通讯结果却缺三层网络和证据图时使用；从单细胞及可用代谢数据推断通讯潜力。只有疾病或发表愿望时先检查问题与数据，不把酶表达当实测代谢流。 |
| `scvi-single-cell-probabilistic-modeling` | 当用户需要使用 scVI、scANVI 或 totalVI 对单细胞计数进行概率表征、半监督标签迁移或 RNA-蛋白联合建模时使用。 |
| `secreted-protein-activity-inference` | 当用户问哪种细胞因子可能让另一群细胞发生变化、某分泌蛋白是否解释接收细胞的基因变化，或已有NicheNet/MultiNicheNet活性结果却缺配体排名和靶基因图时使用；结合发送表达、受体与接收响应推断候选。只有疾病或发表愿望时先检查问题与数据，不直接承诺机制。 |
| `single-cell-alternative-splicing` | 当用户需要从单细胞或单核RNA测序研究外显子、剪接位点、内含子保留和细胞状态相关的可变剪接时使用。 |
| `single-cell-cohort-integration-meta-analysis` | 当用户问换个队列还成立吗、细胞在什么阶段开始变、整合后结论相反，或需多队列单细胞状态复现与元分析（StateShiftAtlas方向）时使用；核验供体、状态和有序轴，自主选择可比较分析，不要求用户认识算法。 |
| `single-cell-genetic-variant-detection` | 当用户想从单细胞数据找突变、判断不同部位细胞是否可能来自同一克隆、寻找遗传差异或祖源证据，或提到Monopogen-Indel时使用；先检查是否有带细胞标识的读段与参考，表达矩阵或伪时间不能替代遗传变异证据。 |
| `single-cell-transposon-expression` | 当用户需要在单细胞 RNA 数据中估计转座元件家族或位点表达，并显式处理重复序列多重比对和基因重叠时使用。 |
| `transcriptomic-reverse-perturbation` | 当用户已有或希望构建两个转录组状态的差异签名，需要利用遗传扰动响应参考库筛选可能模拟或逆转该变化的候选基因扰动，或明确要求用 RevPert 排序并解释候选驱动因子时使用。 |
| `21-biological-foundation-models-b04-t01` | 当用户需要用scGPT为单细胞表达数据生成嵌入、辅助细胞类型注释或构建基因表示时使用。 |

## 空间组学分析（15）

| 技能 | 说明 |
|---|---|
| `he-virtual-spatial-transcriptomics` | 当用户需要用DeepSpot-M从H&E切片切块预测空间基因表达并评估适用性时使用。 |
| `06-spatial-omics-b05-t01` | 当用户需要分析带空间坐标的染色质可及性或空间表观组数据，并识别空间调控区域、细胞状态和区域差异时使用。 |
| `06-spatial-omics-cell2location` | 当用户需要利用匹配的单细胞参考估计空间 spot/bin 的细胞组成，或把细胞状态映射到组织位置，并量化参考缺失与映射不确定性时使用。 |
| `06-spatial-omics-spatial-domain-identification` | 当用户需要根据表达、形态和物理邻接识别组织域与边界，并评估域在样本、尺度和算法之间是否稳定时使用。 |
| `06-spatial-omics-spatial-metabolomics` | 当用户需要处理 MALDI、DESI 等质谱成像数据，建立可信离子图、空间代谢物注释和组织区域比较；适用于保留像素坐标的 MSI 任务时使用。 |
| `06-spatial-omics-spatial-microenvironment` | 当用户问组织里谁挨着谁、肿瘤边缘哪些细胞可能互相影响、某分子信号是否集中在特定位置，或已有空间通讯结果却缺组织定位/邻域网络、图中连线过密，以及需要MISTy空间邻域贡献分析时使用；结合真实空间坐标、细胞组成与配体–受体证据。只有疾病或发表愿望时先检查问题与数据，无坐标不运行空间推断。 |
| `nfcore-molkart` | 当Resolve Molecular Cartography 交付数据需要整理分子坐标与细胞表达时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/molkart。 |
| `nfcore-panoramaseq` | 当已确认原位阵列空间转录测序，需要将读段与空间位置关联时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/panoramaseq。 |
| `nfcore-pixelator` | 当分子邻近测定的 PNA 或 MPX 数据需要分子图和细胞相关分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/pixelator。 |
| `nfcore-sopa` | 当空间图像与分子坐标需要联合分割、聚合和分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/sopa。 |
| `nfcore-spatialaxe` | 当Xenium 或 Artera 交付数据需要检查空间细胞、分子与特征质量时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/spatialaxe。 |
| `nfcore-spatialvi` | 当Visium 计数与组织图像需要联合分析空间表达时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/spatialvi。 |
| `spatial-proteomics` | 当用户需要分析 CODEX、IMC、MIBI 等多通道空间蛋白数据，完成通道校正、细胞分割、表型和组织邻域定量时使用。 |
| `spatial-transcriptomics` | 当用户想知道组织中基因或细胞在哪里、哪些细胞相邻、换半径或分割后结论是否可靠，或交付Visium、Xenium、MERFISH文件及EISTA/SpatialRobust请求时使用；自主识别平台、坐标和阶段，保留spot、bin与细胞边界，不要求用户选择算法。 |
| `21-biological-foundation-models-nicheformer` | 当用户需要用Nicheformer分析空间转录组细胞表征、组织微环境或空间邻域时使用。 |

## 表观遗传与 DNA 甲基化（31）

| 技能 | 说明 |
|---|---|
| `27-aging-longevity-dna-methylation-clock` | 当用户需要用冻结的DNA甲基化时钟计算预测年龄、年龄加速或DunedinPACE衰老速度并评估适用域时使用。 |
| `deeptools` | NGS analysis toolkit. Used for BAM to bigWig conversion, quality control (correlation, PCA, fingerprint plots), heatmaps/feature plots (TSS, peaks), suitable for ChIP-seq, RNA-seq, ATAC-seq visualizat… |
| `03-epigenomics-atac-seq-analysis` | 用于从bulk ATAC-seq FASTQ生成开放染色质峰、差异可及区域和质量诊断；当用户需要处理Tn5切点、共识峰或重复一致性时使用。 |
| `03-epigenomics-chip-seq-histone-analysis` | 用于从组蛋白修饰ChIP-seq的IP与匹配input生成峰或宽域、信号轨道和差异富集结果。 |
| `03-epigenomics-chromatin-loop-detection` | 用于从Hi-C、Micro-C或捕获Hi-C数据检测染色质环，注释增强子—启动子互作并比较互作强度。 |
| `03-epigenomics-cut-run` | 用于处理CUT&RUN或CUT&Tag数据，并针对低背景、短片段、IgG对照和外源校准选择峰调用与归一化策略。 |
| `03-epigenomics-dmr-identification` | 用于在组间识别差异甲基化位点与连续区域，并正确处理覆盖深度、生物学重复、空间相关和协变量。 |
| `03-epigenomics-dnase-seq-analysis` | 用于从DNase-seq数据识别DNase超敏位点、生成切割信号轨道并比较染色质可及性。 |
| `03-epigenomics-enhancer-gene-association` | 当用户问某基因受哪些区域调控、ATAC/ChIP peaks对应哪些基因、想围绕候选基因找调控区域或回应调控机制审稿意见，或需要peakScout双向映射与增强子靶基因证据整合时使用；从实际peaks和参考判断可做的分析，不要求用户认识peak–gene方法。 |
| `03-epigenomics-enhancer-identification` | 用于整合开放染色质与活性标记识别候选增强子；当具备H3K27ac、Mediator或BRD4等连续占据信号时，再按stitching和排序定义超级增强子。 |
| `03-epigenomics-footprinting-analysis` | 用于在开放染色质或ChIP峰中做转录因子基序富集、位点扫描和Tn5/DNase足迹推断。 |
| `03-epigenomics-hi-c-analysis` | 用于从Hi-C成对FASTQ构建接触矩阵，诊断连接产物、有效配对、距离衰减和可支持分辨率。 |
| `03-epigenomics-wgbs-analysis` | 用于处理WGBS或RRBS数据，得到CpG及非CpG甲基化计数、覆盖与转换质量；当用户提供亚硫酸氢盐测序FASTQ时使用。 |
| `chromatin-compartment-tad-analysis` | 用于从经过质控的Hi-C矩阵识别A/B区室、TAD和绝缘边界，并在统一分辨率下比较条件差异。 |
| `chromatin-state-allele-specific-analysis` | 当用户需要用多种组蛋白或可及性信号分割染色质状态，或分析等位基因特异的表观调控差异时使用。 |
| `methylation-array-qc-deconvolution` | 当用户需要处理Illumina甲基化芯片、完成探针与样本质控、归一化、批次检查和细胞比例去卷积时使用。 |
| `nfcore-atacseq` | 当已确认 bulk ATAC-seq 数据，需要分析开放染色质与条件差异时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/atacseq。 |
| `nfcore-callingcards` | 当转录调控记录实验的插入位点或 Calling Cards 读段需要分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/callingcards。 |
| `nfcore-chipseq` | 当已有免疫沉淀测序数据，需要定位蛋白或组蛋白修饰富集区域时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/chipseq。 |
| `nfcore-cutandrun` | 当已知 CUT&RUN 或 CUT&Tag 实验，希望定位染色质靶标时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/cutandrun。 |
| `nfcore-epigenomesegmentation` | 当多种表观信号需要整合为染色质状态时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/epigenomesegmentation。 |
| `nfcore-hic` | 当Hi-C 测序数据需要生成接触矩阵或检查染色质空间结构时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/hic。 |
| `nfcore-hicar` | 当已确认 HiCAR 共测定数据，需要整理染色质接触及相关信号时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/hicar。 |
| `nfcore-methylarray` | 当收到甲基化芯片 IDAT 或相关信号，需要质控与差异甲基化分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/methylarray。 |
| `nfcore-methylong` | 当长读长数据含修饰信号或标签，需要量化 DNA 甲基化时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/methylong。 |
| `nfcore-methylseq` | 当转化化学相关 DNA 测序需要估计甲基化水平时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/methylseq。 |
| `nfcore-mnaseseq` | 当MNase 消化测序数据需要分析核小体位置或占据变化时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/mnaseseq。 |
| `nfcore-sammyseq` | 当已有连续提取的染色质组分测序数据，需要分析组分差异或染色质状态时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/sammyseq。 |
| `epigenetics-drug-response-integration` | 当用户需要联合甲基化、染色质或组蛋白信号与药敏、耐药或剂量反应数据，寻找表观调控型药物响应标志物时使用。 |
| `dna-methylation-wgbs` | \| DNA methylation analysis skill covering two data tracks: bisulfite sequencing (WGBS / RRBS, single-base resolution; upstream Bismark or bwa-meth, downstream methylKit / DSS / bsseq) and enrichment-b… |
| `epigenomics-peak-calling` | \| Epigenomics peak-calling and QC mainline for ChIP-seq, ATAC-seq and CUT&Tag/CUT&RUN: assay triage, alignment (bowtie2/BWA), duplicate handling (Picard MarkDuplicates / samtools markdup), MAPQ and EN… |

## 调控网络与序列模型（18）

| 技能 | 说明 |
|---|---|
| `borzoi` | 使用 Borzoi 根据 DNA 序列预测全基因组功能轨迹（RNA-seq、CAGE、DNase、ChIP）。适用于评估变异对表达或染色质可及性的调控效应、生成某个基因组位点的预测覆盖轨迹，或根据预测轨迹差值确定非编码变异的优先级。 |
| `differential-regulatory-network` | 用于比较疾病与对照、处理前后或细胞状态之间的网络重连；当用户关注边或模块如何变化而非单基因差异时使用。 |
| `evo2` | 使用长上下文基因组基础模型 Evo 2 对 DNA 序列进行评分、嵌入和生成。适用于计算逐核苷酸或逐序列似然以评估变异效应、嵌入基因组窗口供下游分类使用、根据前缀生成 DNA，以及跨物种评估调控区或编码区。 |
| `grn-inference-scaffold-replace` | 用于从表达、染色质可及性或转录因子先验推断基因调控网络；当用户需要TF—靶基因关系或调控模块时使用。 |
| `network-pharmacology-analysis` | 用于整合药物、靶点、疾病基因和通路形成可审计的网络药理学假设；当用户需要候选机制或联合靶点优先级时使用。 |
| `network-topology-community-analysis` | 用于计算生物网络中心性、连通结构、社区和稳健性；当用户已有节点边表并希望寻找模块或关键节点时使用。 |
| `nfcore-diseasemodulediscovery` | 当疾病相关基因及互作网络需要寻找候选疾病模块时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/diseasemodulediscovery。 |
| `sbml-network-modeling` | 用于读取、检查、构建或转换SBML格式的反应网络模型；当用户处理动力学模型、代谢模型交换或模型可重复性时使用。 |
| `string` | 用于从基因或蛋白列表构建、筛选和解释蛋白质互作网络；当用户需要分析PPI、枢纽蛋白或功能模块时使用。 |
| `temporal-gene-regulatory-network` | 用于带时间点或轨迹顺序的表达数据推断动态调控关系；当用户关心调控先后、状态转换或延迟效应时使用。 |
| `wgcna-coexpression-network` | 当用户想找疾病相关的一组协同变化基因、筛枢纽、把RNA与蛋白等组学联系起来、比较模块在不同队列是否稳定，或要求WGCNA/WGCNA+时使用；自主核实样本量、矩阵和配对关系，不能从单个基因或少量细胞假造共表达网络。 |
| `03-epigenomics-basenji` | 用于用Borzoi、Basenji、Enformer、Akita、AlphaGenome等模型预测序列变异对表达、可及性或染色质结构的潜在影响。 |
| `04-transcriptomics-tf-activity-inference` | 用于从表达数据和TF—靶基因regulon推断转录因子活性；当TF自身表达量不足以代表其调控状态时使用。 |
| `nfcore-tfactivity` | 当表达和染色质可及性数据希望推断转录因子活动变化时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/tfactivity。 |
| `single-cell-regulatory-network` | 当用户需要从单细胞 RNA、ATAC 或多组学数据构建带 motif、可及性和扰动支持的 TF-regulon 调控网络时使用。 |
| `21-biological-foundation-models-b01-t03` | 当用户需要用Evo 2对长DNA序列进行似然评分、嵌入、变异效应比较或条件生成时使用。 |
| `plant-long-context-genome-modeling` | 当用户研究水稻、拟南芥等植物的候选基因/调控区域，想比较长DNA片段或变异、寻找可辅助课题的序列模型证据，或指定BOTANIC-1时使用；先确定物种、参考、任务和模型资源，不因植物基因名自动生成预测。 |
| `arboreto` | Infer gene regulatory networks (GRNs) from gene expression data using scalable algorithms (GRNBoost2, GENIE3). Use when analyzing transcriptomics data (bulk RNA-seq, single-cell RNA-seq) to identify t… |

## 蛋白质组学（21）

| 技能 | 说明 |
|---|---|
| `27-aging-longevity-protein-aging-clock` | 当用户需要把冻结的器官特异蛋白质衰老时钟应用到匹配面板的Olink NPX数据并解释年龄加速时使用。 |
| `07-proteomics-dia-proteomics` | 当用户需要处理 DIA-PASEF、SWATH 等数据，选择谱图库或无库搜索，并获得带分层 FDR 和运行质量证据的肽段、蛋白定量时使用。 |
| `07-proteomics-lc-ms-ms` | 当用户需要读取和整理蛋白质组 raw/mzML 数据，完成格式核验、质心与校准检查、谱图或色谱特征处理，为搜索和定量准备输入时使用。 |
| `07-proteomics-phosphorylation` | 当用户需要分析磷酸化、乙酰化、泛素化等翻译后修饰的鉴定、位点定位、丰度变化及其与总蛋白变化的关系时使用。 |
| `07-proteomics-protein-quantification` | 当用户需要把肽段强度、谱图计数或 label-free 信号汇总为可比较的蛋白丰度，并处理跨运行匹配、归一化和缺失时使用。 |
| `07-proteomics-skill-002` | 当用户需要根据蛋白序列及可靠同源证据注释结构域、家族、GO 和功能，同时保留冲突、低覆盖与未知项时使用。 |
| `07-proteomics-tmt-proteomics` | 当用户需要分析 TMT/iTRAQ 等等重标签蛋白质组，处理通道映射、同位素杂质、隔离干扰和跨批次桥接时使用。 |
| `affinity-proteomics-analysis` | 当用户需要分析 Olink、SomaScan 等亲和试剂平台的 NPX/RFU 数据，正确处理板效应、检测限、探针版本和一蛋白多探针时使用。 |
| `nfcore-ddamsproteomics` | 当已有历史 DDA 质谱交付数据，需要评估或复现肽段鉴定与蛋白定量时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/ddamsproteomics。 |
| `nfcore-diaproteomics` | 当已确认 DIA 质谱与谱图库，需要色谱对齐及蛋白定量时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/diaproteomics。 |
| `nfcore-mspepid` | 当已有 MS2 谱图，需要搜索肽段并评估鉴定可靠性时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/mspepid。 |
| `nfcore-proteinannotator` | 当蛋白 FASTA 需要识别结构域或功能特征时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/proteinannotator。 |
| `nfcore-proteinfamilies` | 当多条蛋白序列需要聚类成家族，或向既有家族添加成员时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/proteinfamilies。 |
| `nfcore-proteogenomicsdb` | 当有基因组、转录本或变异材料，需要构建适合质谱搜索的序列库时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/proteogenomicsdb。 |
| `nfcore-proteomicslfq` | 当已有非标记蛋白质组质谱或历史结果，需要评估归档定量流程时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/proteomicslfq。 |
| `nfcore-quantms` | 当定量质谱数据需要区分 DIA、非标记或同位素标签模式并核查历史处理时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/quantms。 |
| `nfcore-ribomsqc` | 当核糖核苷质谱 QC 数据需要检查仪器或批次性能时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/ribomsqc。 |
| `peptide-identification-protein-inference` | 当用户需要从 DDA/DIA MS/MS 谱图完成数据库搜索、分层 FDR 控制和透明的肽段到蛋白群推断时使用。 |
| `proteomics-quality-control` | 当用户需要从仪器、鉴定和定量三个层次定位蛋白质组异常，并给出保留、重跑或剔除样本的证据时使用。 |
| `proteomics-quantification` | 蛋白质组定量下游分析——把 MaxQuant / DIA-NN / Spectronaut / FragPipe 的输出转成可统计的蛋白矩阵，做过滤、归一化、缺失值处理、limma/DEqMS 差异分析、富集与交付。当用户给的是 proteinGroups.txt、report.tsv、peptides.txt 这类定量结果（而不是原始 RAW/mzML）时使用；原始谱图处理与肽段鉴定用 pyop… |
| `pyopenms` | Comprehensive mass spectrometry analysis platform covering both proteomics and metabolomics. PyOpenMS handles proteomics workflows (feature detection, peptide identification, protein quantification, c… |

## 代谢组与脂质糖组（18）

| 技能 | 说明 |
|---|---|
| `tooluniverse-metabolomics` | Comprehensive metabolomics research skill for identifying metabolites, analyzing studies, and searching metabolomics databases. Integrates HMDB (220k+ metabolites), MetaboLights, Metabolomics Workbenc… |
| `08-metabolomics-exposomics` | 当用户需要整合环境化学物、外源代谢物和多来源暴露测量，完成证据分级、单暴露扫描和混合暴露分析时使用。 |
| `08-metabolomics-exposure-biomarker-discovery` | 当用户需要从代谢组数据发现并验证诊断、预后或暴露标志物，重点防止预处理泄漏和只在单一队列有效的过拟合时使用。 |
| `08-metabolomics-flux-analysis` | 当用户需要设计和分析 13C、15N 等示踪实验，校正天然丰度并从同位素体分布推断可识别的代谢流时使用。 |
| `08-metabolomics-icp-ms-analysis` | 当用户需要对 ICP-MS 或 ICP-MS/MS 元素数据进行校准、内标和干扰校正，输出带检测限、回收率与单位的离子组/金属组结果时使用。 |
| `08-metabolomics-metabolite-identification` | 当用户需要整合加合物、同位素、精确质量、MS/MS、保留时间和标准品，为代谢特征给出分级而非过度确定的身份时使用。 |
| `08-metabolomics-targeted-metabolomics` | 当用户需要对 MRM、PRM 或其他标准曲线靶向数据完成峰积分、内标校正和浓度计算，并正确处理定量范围外结果时使用。 |
| `08-metabolomics-untargeted-metabolomics` | 当用户需要将非靶向 LC-MS 或 GC-MS 原始数据转为可追溯的特征矩阵，并用空白、QC 和峰形证据限制假特征时使用。 |
| `ce-ms-metabolomics` | 当用户需要处理毛细管电泳-质谱数据，校正迁移时间并可靠匹配极性和带电代谢物；适用于 CE 特有漂移与毛细管状态问题时使用。 |
| `dda-dia-acquisition-design` | 当用户需要为代谢组和小分子 LC-MS/MS 选择 DDA 或 DIA，并依据色谱峰宽设计循环时间、TopN、窗口与碰撞能时使用。 |
| `ion-mobility-ccs-analysis` | 当用户需要校准 DTIMS、TWIMS 或 TIMS 漂移数据，计算带不确定性的碰撞截面 CCS，并按一致实验条件辅助候选鉴别时使用。 |
| `lipidomics-analysis` | 当用户需要对 LC-MS/MS 脂质数据进行类别感知的鉴定、命名和定量，并明确脂质分子种、sn 位点及双键位置的证据边界时使用。 |
| `metabolomics-normalization-batch-correction` | 当用户需要利用空白、pooled QC、稀释系列和内标清理代谢组特征，校正运行漂移并评估是否保留真实生物变化时使用。 |
| `nfcore-metaboigniter` | 当非靶向代谢组质谱数据需要提峰、对齐与特征注释时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/metaboigniter。 |
| `nmr-metabolomics` | 当用户需要处理一维或多维 NMR 代谢谱，完成频域转换、相位和基线校正、对齐、峰拟合及可追溯定量时使用。 |
| `glycomics` | \| Glycomics data analysis and glycan structure annotation. Covers data-type triage (N-glycan / O-glycan / intact glycopeptide / glycan array / lectin array), GlyTouCan accession lookup, GlycoCT and WU… |
| `lipidomics-annotation` | \| Lipidomics annotation and lipid-specific analysis. Covers LIPID MAPS classification and shorthand notation (species vs molecular species vs sn-position vs double-bond position), MS1 m/z + adduct mat… |
| `metabolomics-profiling` | 代谢组学分析——非靶向 LC/GC-MS 与靶向定量峰表的 QC 过滤、归一化、变换、PCA/PLS-DA/OPLS-DA（含置换验证）、单变量差异、注释置信级、通路富集与交付。当用户给的是峰表（m/z × 样本）、代谢物定量矩阵或 XCMS/MS-DIAL 输出时使用；原始谱图解卷积与谱库匹配用 pyopenms，代谢物数据库查询用 tooluniverse-metabolomics。 |

## 微生物组与宏基因组（38）

| 技能 | 说明 |
|---|---|
| `nfcore-detaxizer` | 当原始序列可能混有宿主、污染物或其他物种，需要筛查或移除目标序列时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/detaxizer。 |
| `microbial-community-metabolic-network` | 用于由MAG或菌株模型构建群落代谢互作网络并分析交叉喂养；当用户研究菌群功能分工或代谢依赖时使用。 |
| `nfcore-bacmodel` | 当细菌基因组及培养背景需要建立代谢网络或预测生长能力时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/bacmodel。 |
| `09-metagenomics-16s-analysis` | 用于从扩增子原始测序数据完成16S或ITS去噪、特征表构建、物种注释和基础质控；当用户提供FASTQ、样本表或询问扩增子分析流程时使用。 |
| `09-metagenomics-amr-gene-analysis` | 用于宏基因组或菌株基因组的耐药基因、耐药突变和移动元件检测；当用户开展AMR监测或风险评估时使用。 |
| `09-metagenomics-host-microbiome-interaction` | 当用户需要把微生物组成或功能与宿主基因、免疫、代谢或临床表型联合分析，并建立可验证互作证据时使用。 |
| `09-metagenomics-humann` | 用于估计宏基因组的基因家族、反应和通路丰度，并拆分物种贡献；当用户询问微生物群落潜在功能组成时使用。 |
| `09-metagenomics-kraken2` | 用于从宏基因组读段估计物种组成；当用户需要在Kraken2/Bracken的快速全读段分类与MetaPhlAn的标记基因谱之间选择或比较时使用。 |
| `09-metagenomics-mag-reconstruction` | 用于宏基因组读段组装、分箱、MAG质量控制、去冗余和分类；当目标是恢复微生物基因组或新物种时使用。 |
| `09-metagenomics-pathway-prediction` | 用于从16S ASV推测基因家族和通路组成；仅当没有宏基因组数据且用户接受预测性结果时使用。 |
| `bgc-identification-classification` | 当用户需要从微生物预测蛋白 FASTA 使用 BGC-Prophet 识别并分类生物合成基因簇时使用；原始核酸序列的基因预测和后续代谢产物结构鉴定不属于本 Skill。 |
| `edna-metabarcoding-analysis` | 用于环境DNA宏条形码数据的物种检出、污染控制和群落比较；当研究对象来自水体、土壤、沉积物或混合环境样本时使用。 |
| `metagenomics-analysis` | 用于把宏基因组研究从原始读段质控串联到物种、功能、耐药和统计解释；当用户需要完整而非单点流程时使用。 |
| `nfcore-ampliseq` | 当报告或引物证据表明是 16S、ITS 等扩增子测序，需要研究微生物群落时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/ampliseq。 |
| `nfcore-bacass` | 当已确认细菌分离株测序，需要组装、修正与基因注释时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/bacass。 |
| `nfcore-bactmap` | 当细菌菌株测序需要参考比对、变异比较或系统发育时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/bactmap。 |
| `nfcore-coproid` | 当古粪便测序需要推断宿主来源并评估污染时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/coproid。 |
| `nfcore-createtaxdb` | 当微生物分析需要适合目标样本与分类工具的数据库时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/createtaxdb。 |
| `nfcore-daamicrobiome` | 当已有微生物计数或丰度表，需要比较条件间差异时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/daamicrobiome。 |
| `nfcore-funcprofiler` | 当宏基因组或宏转录组读段需要估计群落功能组成时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/funcprofiler。 |
| `nfcore-funcscan` | 当微生物组装或 MAG 需要筛查功能基因及天然产物相关候选时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/funcscan。 |
| `nfcore-hgtseq` | 当已有可能涉及宿主与供体的序列数据，需要研究水平转移候选时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/hgtseq。 |
| `nfcore-mag` | 当已确认混合微生物 shotgun 数据，需要组装并恢复微生物基因组时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/mag。 |
| `nfcore-magmap` | 当宏基因组或宏转录组数据需要映射至基因组集合并定量基因时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/magmap。 |
| `nfcore-metatdenovo` | 当宏转录组或宏基因组读段缺少合适参考，需要从头组装与注释时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/metatdenovo。 |
| `nfcore-pathogenepidemiology` | 当已确认特定病原体的测序与采样信息，需要基因组流行病学分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/pathogenepidemiology。 |
| `nfcore-pathogensurveillance` | 当连续采集的病原测序需要群体比较与监测时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/pathogensurveillance。 |
| `nfcore-phageannotator` | 当基因组或宏基因组序列需要查找噬菌体及前噬菌体区域时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/phageannotator。 |
| `nfcore-plasmodiumdrugres` | 当已有疟原虫等位基因表或微单倍型数据，需要汇总耐药相关标记时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/plasmodiumdrugres。 |
| `nfcore-taxprofiler` | 当已确认非扩增子的混合微生物测序，需要识别物种与丰度时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/taxprofiler。 |
| `nfcore-tbanalyzer` | 当结核分枝杆菌复合群测序需要分型及相关标记分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/tbanalyzer。 |
| `nfcore-vipr` | 当已有病毒测序或历史结果，需要复核旧版共识和低频变异分析时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/vipr。 |
| `nfcore-viralmetagenome` | 当非靶向混合样本测序需要发现并重建病毒基因组时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/viralmetagenome。 |
| `nfcore-viralrecon` | 当已确认病毒测序，需要获得共识序列和变异结果时使用。根据文件、实验背景与研究问题判断适配性，选择方法及参数并解释限制；无需用户知道 nf-core/viralrecon。 |
| `strain-tracking-transmission-analysis` | 用于样本间菌株相似性、定植持续性和潜在传播链分析；当用户有纵向、家庭、医院或暴发队列时使用。 |
| `mgm-microbiome-foundation-model` | 当用户已有样本×微生物特征丰度表，并需要使用 MGM 构建语料、预训练、微调、预测、生成或重建时使用；原始读段质控、分类和丰度估计使用宏基因组插件。 |
| `scikit-bio` | Biological data toolkit. Sequence analysis, alignments, phylogenetic trees, diversity metrics (alpha/beta, UniFrac), ordination (PCoA), PERMANOVA, FASTA/Newick I/O, for microbiome analysis. |
| `microbiome-diversity-analysis` | 用于扩增子、宏基因组或物种丰度表的α多样性、β多样性及组间群落差异分析；当用户已有特征表和样本元数据时使用。 |
