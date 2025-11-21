# 📘 Document-Level Dataset  

**Research Phase 1: Literature Review** 

This dataset contains **document-level data** extracted from a multilingual literature review on public-sector design and innovation in Latin America. Each row represents a **single publication**, which may reference one or more innovation units, organizations, projects, or individuals.

For a general overview of the Public Design Collective’s mission and research areas, visit the  
➡️ **Organization Profile:** https://github.com/Public-Design-Collective  
➡️ **Website:** https://publicdesigncollective.com

## 🧭 Dataset Purpose  
This dataset captures the structure and content of the academic and grey literature addressing:

- Public-sector design practices  
- Government innovation labs  
- Project-level initiatives  
- Practitioners and institutional actors  
- Cross-country comparisons  
- Regional trends in public-sector innovation  

It enables descriptive analysis of the literature base and supports cross-linking to higher levels (Institutional, Organizational, Project, Individual) in subsequent datasets.



## 📁 File Included

- **Format:** TSV (tab-separated values)  
- **Unit of analysis:** Publication / Document  
- **Original Source languages:** English, Spanish, Portuguese, French
- **Selected Sources languages:** English, Spanish, Portuguese
- **Time span:** 2007 to 2025



## 📊 Schema & Data Dictionary  
Below is the field-by-field data dictionary using the exact column labels in  
`docLevel_LitReviewAnalysis.tsv`, mapped to the corresponding definitions from the taxonomy.

### **Level 0 — Publication / Source**

| Column Name | Type | Definition | Allowed Values / Examples |
|-------------|------|----------------------------------|----------------------------|
| **ID** | string | Unique document identifier (→ *Document ID*). | `"S40"`, `"E04"` |
| **Language** | categorical | Language of the publication. | `English`, `Spanish`, `Portuguese`, `French` |
| **Document Title** | string | Full title of the publication (→ *Title*). | `"Innovation labs in South American governments"` |
| **Citation** | string | Full bibliographic reference for the document. | `"Silva Jr. & Emmendoerfer (2023)...“` |
| **Document Link** | string (URL) | URL to the source document. | `"https://doi.org/..."` |
| **Research objective (LLM)** | string | AI-generated summary of the main research objective | `"Examines how design is used in public innovation"` |
| **Research method (LLM)** | string | AI-inferred methodological classification. | `"Qualitative case study"` |
| **Main conclusions (LLM)** | string | AI-generated summary of key conclusions. | `"Finds that design capacity varies significantly by region"` |
| **Year of Publication** | integer | Year when the document was published. | `2021`, `2023` |
| **Scope of Paper** | categorical | Indicates whether the paper focuses on a single country or multiple. | `Single-country`, `Multi-country` |
| **Specific Latin America Countries Cited** | string (list or comma-separated) | Latin American countries analyzed or referenced. | `"Brazil"`, `"Chile; Colombia; Mexico"` |
| **Country Count** | integer | Number of countries referenced in the document. | `1`, `3`, `7` |
| **Type of Document** | categorical | Nature of the publication. | `Peer-Reviewed Article`, `Report`, `Thesis` |
| **Categories of Topics Discussed** | string (list or categorical) | Main thematic areas. | `"Public Innovation Overview"`, `"Need for initiatives in public innovation"` |
| **Research Methods** | string (list or categorical) | Methods used in the document research. | `"Interviews"`, `"Surveys"`, `"Case Study"` |
| **Count of Innovation Units** | integer | Number of innovation labs referenced in the document. | `0`, `2`, `5` |
| **Count of Organizations** | integer | Number of organizations referenced in the document. | `1`, `4` |
| **Count of Projects** | integer | Number of projects or initiatives mentioned. | `0`, `3` |
| **Count of Individuals** | integer | Number of practitioners/actors named. | `1`, `7` |



