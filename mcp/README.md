# MCP 工具（51）

`biomedical_mcp.py` 是一个 stdio MCP server：一行一条 JSON-RPC 2.0 消息，
只依赖 Python 标准库（`json` / `sys` / `urllib` / `gzip`），不需要 API key、token 或第三方包。

## 启动

```bash
python mcp/biomedical_mcp.py
```

由 MCP 客户端以 stdio 方式拉起即可，通常不需要手动运行。

## 工具清单

工具名格式为 `<域>_<动作>`。共 51 个，覆盖 22 个数据域。

### Ensembl BioMart（2）

| 工具 | 说明 |
|---|---|
| `biomart_query` | Ensembl BioMart ͨ�ò�ѯ��XML over GET���Զ�������ת�������� TSV �С� |
| `biomart_gene_info` | BioMart ���������ȡ����ע�ͣ�Ensembl/Entrez/λ��/biotype/�������� |

### ZINC（1）

| 工具 | 说明 |
|---|---|
| `zinc_search_by_structure` | �� InChIKey �� SMILES �� ZINC��ZINC ���� JSON �ӿ�������ʱ�Զ����� PubChem�� |

### PubMed（3）

| 工具 | 说明 |
|---|---|
| `pubmed_search_articles` | PubMed �������ף�NCBI E-utilities�������� PMID�����⡢�ڿ������ڡ����ߡ�DOI�� |
| `pubmed_get_article_metadata` | �� PMID ȡ����Ԫ���ݣ��� DOI/PMCID���� |
| `pubmed_find_related` | �� PMID �� PubMed �����������ס� |

### ChEMBL（3）

| 工具 | 说明 |
|---|---|
| `chembl_compound_search` | ChEMBL ������������������� ChEMBL ID��SMILES���з��׶Ρ� |
| `chembl_get_bioactivity` | ȡĳ��������е��ʵ����ԣ�IC50/Ki �ȣ��� |
| `chembl_target_search` | �����ƻ����������� ChEMBL �е㡣 |

### bioRxiv（2）

| 工具 | 说明 |
|---|---|
| `biorxiv_get_preprint` | �� DOI ȡ bioRxiv/medRxiv Ԥӡ��Ԫ���ݣ���ͬ�����飩�� |
| `biorxiv_recent_preprints` | ������������Ԥӡ���� |

### ClinicalTrials.gov（2）

| 工具 | 说明 |
|---|---|
| `clinicaltrials_search_trials` | ClinicalTrials.gov v2 ��������� |
| `clinicaltrials_get_trial` | �� NCT ��ȡ���������¼�� |

### 基因组序列与注释（3）

| 工具 | 说明 |
|---|---|
| `genomes_ensembl_lookup` | Ensembl ��������Ż��ȶ� ID ��ע�ͣ�λ�á�biotype��ת¼������ |
| `genomes_ensembl_sequence` | ȡ���У��� region ȡ���䣬��� stable_id ȡ�� ID ���С� |
| `genomes_ensembl_overlap` | ��ĳ�������ص��Ļ���/ת¼���������� |

### 变异数据库（3）

| 工具 | 说明 |
|---|---|
| `variants_gnomad_get_variant` | gnomAD v4 �����Ⱥ��Ƶ�ʣ���������(429)���Զ����˵� Ensembl ��ȺƵ�ʡ� |
| `variants_clinvar_search` | ClinVar ������NCBI E-utilities���� |
| `variants_dbsnp_get` | dbSNP �� rsID ȡ��¼ժҪ�� |

### 表达数据（2）

| 工具 | 说明 |
|---|---|
| `expression_gtex_median` | GTEx ĳ�������֯��λ���TPM�����򣩡��� GENCODE ID�� |
| `expression_gtex_tissue_sites` | �� GTEx ��֯λ�㡣 |

### 调控与表观（2）

| 工具 | 说明 |
|---|---|
| `regulation_encode_search` | ENCODE ����ʵ�飻��վ�����ɴʧ�ܿɴ� region ���˵� Ensembl �������� |
| `regulation_jaspar_matrix` | JASPAR ���󣺸� matrix_id ȡ���飬�򰴹ؼ��ʼ����� |

### 蛋白注释（3）

| 工具 | 说明 |
|---|---|
| `protein_annotation_interpro_domains` | InterPro ȡ UniProt ���׵Ľṹ��ܹ��� |
| `protein_annotation_string_network` | STRING v12 ȡ���׻������硣 |
| `protein_annotation_hpa_gene` | Human Protein Atlas ��������ȡ��¼�� |

### 结构（3）

| 工具 | 说明 |
|---|---|
| `structures_pdb_entry` | RCSB PDB �� PDB ID ȡ��ĿժҪ�� |
| `structures_pdb_search` | RCSB PDB ȫ�ļ����� |
| `structures_alphafold_prediction` | AlphaFold DB ȡ UniProt ��Ԥ��ṹ���ӡ� |

### RNA（2）

| 工具 | 说明 |
|---|---|
| `rna_rfam_family` | Rfam �������飨accession�����͡�seed/full �������� |
| `rna_rfam_search` | Rfam �ؼ��ʼ����� |

### 基因注释（3）

| 工具 | 说明 |
|---|---|
| `genes_ontologies_mygene_query` | MyGene ���������������/ID�� |
| `genes_ontologies_quickgo_annotations` | QuickGO ȡ UniProt ���׵� GO ע�͡� |
| `genes_ontologies_ols_term` | OLS4 ȡ�����������顣 |

### 多组学（3）

| 工具 | 说明 |
|---|---|
| `omics_archives_geo_search` | GEO �������ݼ���NCBI gds���� |
| `omics_archives_pride_project` | PRIDE �� accession ȡ����������Ŀ�� |
| `omics_archives_biostudies_search` | BioStudies/ArrayExpress ������ |

### 人类本体（1）

| 工具 | 说明 |
|---|---|
| `human_genetics_variant_phenotypes` | �� rsID ȡ�����������״�� p ֵ��Ensembl variation��GWAS Catalog �� REST �����ߣ��� |

### 癌症（2）

| 工具 | 说明 |
|---|---|
| `cancer_models_cbioportal_studies` | ��/ɸ cBioPortal �о��� |
| `cancer_models_cbioportal_mutations` | ȡĳ�о���ĳ�����ͻ�䣨�Զ��������о���ͻ������ף��� |

### 单细胞图谱（2）

| 工具 | 说明 |
|---|---|
| `cellguide_cellxgene_collections` | CELLxGENE Discover �й������ݼ����ϡ� |
| `cellguide_search_cell_types` | �����Ƽ��� Cell Ontology ϸ�����ͣ�OLS4/CL�������� CL ID �������� |

### 化学（3）

| 工具 | 说明 |
|---|---|
| `chemistry_pubchem_search` | PubChem ������/SMILES/InChIKey ���� CID�� |
| `chemistry_pubchem_properties` | PubChem �� CID ȡ�������ԡ� |
| `chemistry_rhea_reaction` | Rhea ����Ӧ ID ȡ����ʽ������ߡ� |

### 临床（2）

| 工具 | 说明 |
|---|---|
| `clinical_genomics_civic_search` | CIViC GraphQL ������֢֤����Ŀ�� |
| `clinical_genomics_opentargets_disease_targets` | Open Targets ȡ���������е㡣 |

### 药物（2）

| 工具 | 说明 |
|---|---|
| `drug_regulatory_openfda_labels` | openFDA ����ҩƷ˵���顣 |
| `drug_regulatory_openfda_drugsfda` | openFDA Drugs@FDA ���������¼�� |

### 文献计量（2）

| 工具 | 说明 |
|---|---|
| `literature_graph_openalex_search` | OpenAlex ��ѧ�����׼����� |
| `literature_graph_arxiv_search` | arXiv ���������� Atom XML Ƭ�Σ��� |

## 说明

- 所有工具直连公开 REST API（NCBI E-utilities、Ensembl、UniProt、PDB、ChEMBL、ClinicalTrials.gov 等），不经任何网关。
- 无鉴权：受各自站点未授权访问速率限制，高频调用请自行加间隔。
- 部分工具在源站失败时会自动降级到等价来源（例如 gnomAD 限流时改取 Ensembl 区域变异）。
