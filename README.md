


# Awesome Data Discovery and Observability [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

This repository contains a curated list of awesome data catalogs and observability platforms that help you discover, manage, and observe data in your organization. 

<br>

## Contents: Data Discovery and Observability Solutions

| [OSS Data Catalogs](#opensource)             | [ Proprietary Cloud DCs](#monocloud)       | [ Proprietary Observability Tools](#observability) | [Other Proprietary DCs](#proprietary) |
|----------------------------------------------|--------------------------------------------|---------------------------------|--------------------------------|
| [📙 Amundsen](#amundsen)                     | [📒 Amazon DataZone](#aws)                 | [🔍 Monte Carlo](#montecarlo)  | [📕 Alation](#alation)         |
| [📙 DataHub](#datahub)                       | [📒 Google Cloud Dataplex](#google)        | [🔍 Databand](#databand)       | [📕 Atlan](#atlan)             |
| [📙 Marquez](#marquez)                       | [📒 Microsoft Purview](#azure)             | [🔍 Datafold](#datafold)       | [📕 Collibra](#collibra)       |
| [📙 Atlas](#atlas)                           | [📒 Databricks Unity Catalog](#databricks) | [🔍 Ataccama](#ataccama)       | [📕 DataGalaxy](#datagalaxy) |
| [📙 CKAN](#ckan)                             | [📒 Snowflake Horizon Catalog](#snowflake) | [🔍 DataKitchen Open Source Data Observability](#datakitchen)| [📕 Informatica](#informatica) |
| [📙 Magda](#magda)                           |                                            |                                | [📕 Stemma](#stemma)          |
| [📙 Open Data Discovery](#opendatadiscovery) |                                            |                                | [📕 Talend](#talend) |
| [📙 OpenMetadata](#openmetadata)             |                                            |                                | [📕 Select Star](#selectstar) |
| [📙 Elementary](#elementary)                 |                                            |                                | |
| [📙 Gravitino](#gravitino)                   |                                            |                                | |
| [📙 Soda Core](#soda)                        |                                            |                                | |
| [📙 Meta\#Grid](#metagrid)                   |                                            |                                | |
| [📙 Grai](#grai)                             |                                            |                                | |
| [📙 Hamilton](#hamilton)                     |                                            |                                | |
| [📙 Egeria](#egeria)                         |                                            |                                | |

<br>

---

## GenAI Readiness Features

As Generative AI (GenAI) solutions gain prominence, the role of robust Metadata Management Systems equipped with Large Language Model (LLM) capabilities becomes increasingly critical. Such systems significantly enhance context-awareness, enabling advanced semantic understanding, bridging the gap between business and technical metadata, and effectively powering Retrieval-Augmented Generation (RAG) and Agent-to-Agent (A2A) interactions. We observe a notable convergence where RAG systems, initially context-limited, incorporate Metadata Management capabilities, while Metadata Management platforms increasingly adopt GenAI functionalities to cater to new, sophisticated use-cases.

The following categories outline key GenAI readiness features available across various Metadata Management solutions:

* AI & Semantic Metadata Enrichment
* Semantic Translation & Business Glossaries
* Technical Metadata & Query Analytics
* Data Quality, Observability & Governance

> **Disclaimer:**
> The GenAI feature landscape evolves rapidly, and thus the provided list, feature groupings, and matrix may frequently change. Contributions, updates, and community-driven insights are strongly encouraged to keep this resource comprehensive and current.

---

### AI & Semantic Metadata Enrichment

The group includes built-in AI capabilities essential for Generative AI applications, enhancing metadata through semantic enrichment and context awareness. It supports Agent-to-Agent (A2A) protocols and Retrieval-Augmented Generation (RAG) systems by facilitating semantic understanding, vectorization, and natural language interactions.

| Product                           | Vendor / Origin                            | Offering Type | GitHub Repo                                                                 | Official Website                                                      | MCP Support | GenAI Metadata Enrichment | Classic ML Metadata Enrichment | Built-in AI Assistant | Semantic Search | Vector Store Collector | API Access |
|-----------------------------------|--------------------------------------------|---------------|------------------------------------------------------------------------------|------------------------------------------------------------------------|-------------|--------------------------|--------------------------|------------------------|------------------|--------------------------|-------------|
| Open Data Discovery               | Provectus / Community                      | OSS           | [GitHub](https://github.com/opendatadiscovery/odd-platform)                | [opendatadiscovery.org](https://opendatadiscovery.org)               | ❌           | ❌️                        | ✔️                        | ❌                      | ❌                | ✔️                        | ✔️           |
| OpenMetadata                     | OpenMetadata Community (Collate, ex‑Atlas) | OSS           | [GitHub](https://github.com/open-metadata/OpenMetadata)                   | [open-metadata.org](https://open-metadata.org)                        | ✔️           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Amundsen                         | Lyft                                       | OSS           | [GitHub](https://github.com/amundsen-io/amundsen)                         | [amundsen.io](https://www.amundsen.io)                                | ❌           | ❌️                       | ❌️                       | ❌                      | ✔️               | ?                        | ✔️           |
| DataHub                          | LinkedIn / Community                       | OSS           | [GitHub](https://github.com/datahub-project/datahub)                      | [datahubproject.io](https://datahubproject.io)                        | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ?                        | ✔️           |
| Marquez                          | WeWork / LF AI & Data                      | OSS           | [GitHub](https://github.com/MarquezProject/marquez)                       | [marquezproject.ai](https://marquezproject.ai)                        | ❌           | ❌                       | ❌                       | ❌                      | ❌               | ❌                       | ✔️           |
| Gravitino                        | Apache Software Foundation                 | OSS           | [GitHub](https://github.com/apache/incubator-gravitino)                   | [gravitino](https://incubator.apache.org/projects/gravitino.html)     | ❌           | ❌                       | ❌                       | ❌                      | ❌               | ❌                       | ✔️           |
| Soda Core                        | Soda                                       | OSS           | [GitHub](https://github.com/sodadata/soda-core)                           | [soda.io](https://soda.io)                                            | ❌           | ❌                       | ❌                       | ❌                      | ❌               | ❌                       | ✔️           |
| Elementary                       | Elementary Data                            | OSS           | [GitHub](https://github.com/elementary-data/elementary)                   | [elementary-data.com](https://elementary-data.com)                    | ❌           | ❌                       | ❌                       | ❌                      | ❌               | ❌                       | ✔️           |
| Egeria                           | LF / ODPi                                  | OSS           | [GitHub](https://github.com/odpi/egeria)                                  | [egeria.odpi.org](https://egeria.odpi.org)                            | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ?                        | ✔️           |
| Magda                            | CSIRO / Community                          | OSS           | [GitHub](https://github.com/magda-io/magda)                               | [magda.io](https://magda.io)                                          | ❌           | ❌                       | ❌                       | ❌                      | ✔️               | ❌                       | ✔️           |
| Atlas                            | Apache Software Foundation                 | OSS           | [GitHub](https://github.com/apache/atlas)                                 | [atlas.apache.org](https://atlas.apache.org)                          | ❌           | ❌                       | ❌                       | ❌                      | ✔️               | ❌                       | ✔️           |
| CKAN                             | Datopian / Link Digital                    | OSS           | [GitHub](https://github.com/ckan/ckan)                                    | [ckan.org](https://ckan.org)                                          | ❌           | ❌                       | ❌                       | ❌                      | ❌               | ❌                       | ✔️           |
| Hamilton                         | Apache / DagWorks                          | OSS           | [GitHub](https://github.com/dagworks-inc/hamilton)                        | [dagworks.io/hamilton](https://www.dagworks.io/hamilton)              | ❌           | ❌                       | ❌                       | ❌                      | ❌               | ❌                       | ✔️           |
| Acryl Data (SaaS Datahub)        | Acryl                                      | Prop          | –                                                                          | [acryl.io](https://www.acryl.io)                                      | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Collate AI Platform              | Collate / SaaS version of OpenMetadata     | Prop          | –                                                                          | [getcollate.io](https://www.getcollate.io/)                                  | ✔️           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Atlan                            | Atlan /                                    | Prop          | [GitHub](https://github.com/atlanhq/atlan)                                | [atlan.com](https://atlan.com)                                        | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Ataccama                         | Ataccama                                   | Prop          | –                                                                          | [ataccama.com](https://www.ataccama.com)                              | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Monte-Carlo                      | Monte Carlo                                | Prop          | –                                                                          | [montecarlo.com](https://www.montecarlo.com)                          | ❌           | ✔️                       | ✔️                       | ❌                      | ❌               | ❌                       | ✔️           |
| Select Star                      | Select Star                                | Prop          | –                                                                          | [selectstar.com](https://www.selectstar.com)                          | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ?                        | ✔️           |
| OvalEdge Data Catalog            | OvalEdge                                   | Prop          | –                                                                          | [ovaledge.com](https://www.ovaledge.com)                              | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Datakin                          | Datakin                                    | Prop          | [GitHub](https://github.com/datakin)                                      | [datakin.com](https://datakin.com)                                    | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ?                        | ✔️           |
| Alation Data Catalog             | Alation                                    | Prop          | –                                                                          | [alation.com](https://www.alation.com)                                | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Informatica Data Catalog         | Informatica                                | Prop          | –                                                                          | [informatica.com](https://www.informatica.com)                        | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Precisely Data Integrity Suite   | Precisely                                  | Prop          | –                                                                          | [precisely.com](https://www.precisely.com)                            | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ?                        | ✔️           |
| erwin Data Intelligence          | Quest                                      | Prop          | –                                                                          | [quest.com](https://www.quest.com/products/erwin-data-intelligence)   | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ✔️                       | ✔️           |
| OneTrust Data Discovery          | OneTrust                                   | Prop          | –                                                                          | [onetrust.com](https://www.onetrust.com/products/data-discovery)      | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ✔️                       | ✔️           |
| Collibra Data Catalog            | Collibra                                   | Prop          | [GitHub](https://github.com/collibra)                                     | [collibra.com](https://www.collibra.com)                              | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| data.world Data Catalog Platform | data.world / ServiceNow                    | Prop          | [GitHub](https://github.com/datadotworld)                                 | [data.world](https://data.world)                                      | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Zeenea Data Catalog              | Zeenea                                     | Prop          | [GitHub](https://github.com/zeenea)                                       | [zeenea.com](https://www.zeenea.com)                                  | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ?                        | ✔️           |
| Explorium                        | Explorium                                  | Prop          | [GitHub](https://github.com/explorium-ai)                                 | [explorium.ai](https://www.explorium.ai)                              | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Talend                           | Talend                                     | Prop          | –                                                                          | [talend.com](https://www.talend.com)                                  | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ✔️                       | ✔️           |
| Metaplane                        | Metaplane                                  | Prop          | –                                                                          | [metaplane.com](https://www.metaplane.com)                            | ❌           | ✔️                       | ✔️                       | ❌                      | ✔️               | ❌                       | ✔️           |
| BigID Data Intelligence Platform | BigID                                      | Prop          | –                                                                          | [bigid.com](https://www.bigid.com)                                    | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| IBM watsonx.data intelligence    | IBM                                        | Prop          | –                                                                          | [ibm.com](https://www.ibm.com/products/watsonx-data)                  | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Databricks Unity Catalog         | Databricks                                 | Cloud         | –                                                                          | [databricks.com](https://www.databricks.com/product/unity-catalog)    | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Snowflake Horizon Catalog        | Snowflake                                  | Cloud         | –                                                                          | [snowflake.com](https://www.snowflake.com/en/data-cloud/horizon)     | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| AWS DataZone                     | AWS                                        | Cloud         | –                                                                          | [aws.amazon.com](https://aws.amazon.com/datazone)                     | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Google Cloud Dataplex            | Google Cloud                               | Cloud         | –                                                                          | [cloud.google.com/dataplex](https://cloud.google.com/dataplex)        | ❌           | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |
| Microsoft Purview                | Microsoft                                  | Cloud         | –                                                                          | [azure.microsoft.com](https://azure.microsoft.com/en-us/products/purview) | ❌       | ✔️                       | ✔️                       | ✔️                     | ✔️               | ✔️                       | ✔️           |


### Semantic Translation & Business Glossaries

Features enabling a semantic bridge between business concepts and technical metadata. These capabilities enable precise mapping between business terms and data assets, fostering accurate, context-aware query generation.

| Product                            | Vendor / Origin                                     | Offering Type | GitHub Repo                                                                 | Official Website                                       | Data Asset Level Business Name | Column Level Business Name | Data Asset Level Description | Column Level Description | Data Asset Level Tagging | Column Level Tagging | Business Glossary | Glossary to Data Asset Lineage | Glossary to Column Lineage | Glossary to Glossary Lineage | Glossary to Query Example Lineage |
|------------------------------------|-----------------------------------------------------|----------------|------------------------------------------------------------------------------|---------------------------------------------------------|-------------------------------|----------------------------|------------------------------|---------------------------|--------------------------|-----------------------|--------------------|-------------------------------|----------------------------|------------------------------|-----------------------------------|
| Open Data Discovery                | Provectus / Community                               | OSS            | [GitHub](https://github.com/opendatadiscovery/odd-platform)               | [opendatadiscovery.org](https://opendatadiscovery.org) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ?                                 |
| OpenMetadata                       | OpenMetadata Community (Collate, ex-Atlas/Databook) | OSS            | [GitHub](https://github.com/open-metadata/OpenMetadata)                   | [open-metadata.org](https://open-metadata.org)         | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ?                                 |
| Amundsen                           | Lyft                                                | OSS            | [GitHub](https://github.com/amundsen-io/amundsen)                         | [amundsen.io](https://www.amundsen.io)                 | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ?                          | ?                            | ?                                 |
| DataHub                            | LinkedIn-origin / DataHub Project                   | OSS            | [GitHub](https://github.com/datahub-project/datahub)                      | [datahubproject.io](https://datahubproject.io)         | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ?                                 |
| Marquez                            | WeWork-origin / LF AI & Data                        | OSS            | [GitHub](https://github.com/MarquezProject/marquez)                       | [marquezproject.ai](https://marquezproject.ai)         | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Gravitino                          | Apache Software Foundation                          | OSS            | [GitHub](https://github.com/apache/incubator-gravitino)                   | [Apache Gravitino](https://incubator.apache.org/projects/gravitino.html) | ❌                            | ❌                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Soda Core                          | Soda                                                | OSS            | [GitHub](https://github.com/sodadata/soda-core)                           | [soda.io](https://soda.io)                             | ❌                            | ❌                         | ❌                           | ❌                        | ❌                       | ❌                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Elementary                         | Elementary Data                                     | OSS            | [GitHub](https://github.com/elementary-data/elementary)                   | [elementary-data.com](https://elementary-data.com)     | ❌                            | ❌                         | ❌                           | ❌                        | ❌                       | ❌                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Egeria                             | LF / ODPi                                           | OSS            | [GitHub](https://github.com/odpi/egeria)                                   | [egeria.odpi.org](https://egeria.odpi.org)             | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ?                                 |
| Magda                              | magda.io / CSIRO-origin                             | OSS            | [GitHub](https://github.com/magda-io/magda)                               | [magda.io](https://magda.io)                           | ✔️                            | ?                          | ✔️                           | ?                         | ✔️                       | ❌                    | ✔️                 | ❌                            | ❌                         | ?                            | ❌                                |
| Atlas                              | Apache Software Foundation                          | OSS            | [GitHub](https://github.com/apache/atlas)                                 | [atlas.apache.org](https://atlas.apache.org)           | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ❌                                |
| CKAN                               | Datopian / Link Digital                             | OSS            | [GitHub](https://github.com/ckan/ckan)                                    | [ckan.org](https://ckan.org)                           | ✔️                            | ❌                         | ✔️                           | ❌                        | ✔️                       | ❌                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Hamilton                           | Apache Software Foundation                          | OSS            | [GitHub](https://github.com/dagworks-inc/hamilton)                        | [dagworks.io/hamilton](https://dagworks.io/hamilton)   | ❌                            | ❌                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Acryl Data (SaaS Datahub)          | -                                                   | Prop           | -                                                                          | [acryl.io](https://acryl.io)                           | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Collate AI Platform                | Collate / SaaS version of OpenMetadata              | Prop           | -                                                                          | [collate.io](https://www.getcollate.io/)                       | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Atlan                              | -                                                   | Prop           | [GitHub](https://github.com/atlanhq)                                      | [atlan.com](https://atlan.com)                         | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Ataccama                           | -                                                   | Prop           | -                                                                          | [ataccama.com](https://ataccama.com)                   | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Monte-Carlo                        | -                                                   | Prop           | -                                                                          | [montecarlo.com](https://montecarlo.com)               | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ❌                 | ❌                            | ❌                         | ❌                           | ❌                                |
| Select Star                        | -                                                   | Prop           | -                                                                          | [selectstar.com](https://selectstar.com)               | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| OvalEdge Data Catalog              | -                                                   | Prop           | -                                                                          | [ovaledge.com](https://ovaledge.com)                   | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Datakin                            | -                                                   | Prop           | [GitHub](https://github.com/datakin)                                      | [datakin.com](https://datakin.com)                     | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ?                            | ?                                 |
| Alation Data Catalog               | -                                                   | Prop           | -                                                                          | [alation.com](https://alation.com)                     | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Informatica Data Catalog           | -                                                   | Prop           | -                                                                          | [informatica.com](https://informatica.com)             | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Precisely Data Integrity Suite     | Precisely                                           | Prop           | -                                                                          | [precisely.com](https://precisely.com)                 | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ?                                 |
| erwin Data Intelligence            | Quest                                               | Prop           | -                                                                          | [quest.com](https://quest.com/products/erwin-data-intelligence) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| OneTrust Data Discovery            | OneTrust                                            | Prop           | -                                                                          | [onetrust.com](https://onetrust.com/products/data-discovery) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Collibra Data Catalog              | -                                                   | Prop           | [GitHub](https://github.com/collibra)                                     | [collibra.com](https://collibra.com)                   | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| data.world Data Catalog Platform   | ServiceNow                                          | Prop           | [GitHub](https://github.com/datadotworld)                                 | [data.world](https://data.world)                       | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Zeenea Data Catalog                | -                                                   | Prop           | [GitHub](https://github.com/zeenea)                                       | [zeenea.com](https://zeenea.com)                       | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Explorium                          | -                                                   | Prop           | [GitHub](https://github.com/explorium-ai)                                 | [explorium.ai](https://explorium.ai)                   | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Talend                             | -                                                   | Prop           | -                                                                          | [talend.com](https://talend.com)                       | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Metaplane                          | -                                                   | Prop           | -                                                                          | [metaplane.com](https://metaplane.com)                 | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ❌                                |
| BigID Data Intelligence Platform   | -                                                   | Prop           | -                                                                          | [bigid.com](https://bigid.com)                         | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| IBM watsonx.data intelligence      | IBM                                                 | Prop           | -                                                                          | [ibm.com](https://ibm.com/products/watsonx-data)       | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Databricks Unity Catalog           | Databricks                                          | Cloud          | -                                                                          | [databricks.com](https://databricks.com/product/unity-catalog) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Snowflake Horizon Catalog          | Snowflake                                           | Cloud          | -                                                                          | [snowflake.com](https://snowflake.com/en/data-cloud/horizon) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| AWS DataZone                       | AWS                                                 | Cloud          | -                                                                          | [aws.amazon.com/datazone](https://aws.amazon.com/datazone) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Google Cloud Dataplex              | Google Cloud                                        | Cloud          | -                                                                          | [cloud.google.com/dataplex](https://cloud.google.com/dataplex) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |
| Microsoft Purview                  | Microsoft                                           | Cloud          | -                                                                          | [azure.microsoft.com/purview](https://azure.microsoft.com/en-us/products/purview) | ✔️                            | ✔️                         | ✔️                           | ✔️                        | ✔️                       | ✔️                    | ✔️                 | ✔️                            | ✔️                         | ✔️                           | ✔️                                |


### Technical Metadata & Query Analytics

Core features providing detailed technical insights, query analytics, and usage patterns critical for metadata-informed query generation, optimization, and efficient GenAI-driven data interactions. Essential for automated database query generation, lineage tracking, and metadata-informed GenAI processes.

| Product                           | Vendor / Origin                                                                                                     | Offering Type   | GitHub Repo   | Official Website                                            | Data Asset Level Technical (Source) Name   | Column Level Technical (Source) Name   | Column Data Type   | Column Level Constraints   | Data Asset Relationships (Data Model)   | Data Asset Level Lineage   | Column Level Lineage   | Data Asset Level Metadata Versioning & History   | Column Level Metadata Versioning & History   | Curated Query Examples   | Most Frequent Queries   | Recent Queries   | Data Sample   |
|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------|:----------------|:--------------|:------------------------------------------------------------|:-------------------------------------------|:---------------------------------------|:-------------------|:---------------------------|:----------------------------------------|:---------------------------|:-----------------------|:-------------------------------------------------|:---------------------------------------------|:-------------------------|:------------------------|:-----------------|:--------------|
| Open Data Discovery               | Provectus / Community                                                                                               | OSS             | Github        | opendatadiscovery.org                                       | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| OpenMetadata                      | OpenMetadata Community (founded by Collate & ex‑Atlas/Databook leaders)                                             | OSS             | Github        | open-metadata.org                                           | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Amundsen                          | Lyft                                                                                                                | OSS             | Github        | amundsen.io                                                 | ✔️                                         | ✔️                                     | ✔️                 | ?                          | ✔️                                      | ✔️                         | ?                      | ?                                                | ?                                            | ✔️                       | ✔️                      | ✔️               | ✔️            |
| DataHub                           | LinkedIn‑origin / DataHub Project                                                                                   | OSS             | Github        | datahubproject.io                                           | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Marquez                           | WeWork‑origin / LF AI & Data                                                                                        | OSS             | Github        | marquezproject.ai                                           | ✔️                                         | ✔️                                     | ✔️                 | ?                          | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ❌                       | ?                       | ?                | ❌            |
| Gravitino                         | Apache Software Foundation                                                                                          | OSS             | Githib        | incubator.apache.org/projects/gravitino.html                | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ❌                         | ❌                     | ❌                                               | ❌                                           | ❌                       | ❌                      | ❌               | ❌            |
| Soda Core                         | Soda                                                                                                                | OSS             | Github        | soda.io                                                     | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ❌                                      | ❌                         | ❌                     | ❌                                               | ❌                                           | ❌                       | ❌                      | ❌               | ✔️            |
| Elementary                        | Elementary Data                                                                                                     | OSS             | Github        | elementary-data.com                                         | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ❌                                      | ✔️                         | ✔️                     | ❌                                               | ❌                                           | ❌                       | ❌                      | ❌               | ❌            |
| Egeria                            | LF / ODPi                                                                                                           | OSS             | Github        | egeria.odpi.org                                             | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ?                        | ?                       | ?                | ✔️            |
| Magda                             | magda.io / CSIRO‑origin                                                                                             | OSS             | Github        | magda.io                                                    | ✔️                                         | ?                                      | ✔️                 | ❌                         | ❌                                      | ❌                         | ❌                     | ❌                                               | ❌                                           | ❌                       | ✔️                      | ✔️               | ✔️            |
| Atlas                             | Apache Software Foundation                                                                                          | OSS             | Github        | atlas.apache.org                                            | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ❌                       | ❌                      | ❌               | ❌            |
| CKAN                              | Datopian and Link Digital are co-stewards of the CKAN project and some of the longest standing contributors to CKAN | OSS             | Github        | ckan.org                                                    | ✔️                                         | ❌                                     | ✔️                 | ❌                         | ❌                                      | ❌                         | ❌                     | ✔️                                               | ❌                                           | ❌                       | ❌                      | ❌               | ✔️            |
| Hamilton                          | Apache Software Foundation                                                                                          | OSS             | Github        | dagworks.io/hamilton                                        | ✔️                                         | ✔️                                     | ✔️                 | ❌                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ❌                       | ❌                      | ❌               | ❌            |
| Acryl Data (SaaS Datahub)         | -                                                                                                                   | Prop            | -           | acryl.io                                                    | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Collate AI Platform               | Collate / SaaS version of OpenMetadata                                                                              | Prop            | -           | getcollate.io                                   | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Atlan                             | -                                                                                                                   | Prop            | Github        | atlan.com                                                   | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Ataccama                          | -                                                                                                                   | Prop            | -           | ataccama.com                                                | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Monte-Carlo                       | -                                                                                                                   | Prop            | -           | montecarlo.com                                              | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ❌                       | ❌                      | ❌               | ❌            |
| Select Star                       | -                                                                                                                   | Prop            | -           | selectstar.com                                              | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| OvalEdge Data Catalog             | -                                                                                                                   | Prop            | -           | ovaledge.com                                                | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Datakin                           | -                                                                                                                   | Prop            | Github        | datakin.com                                                 | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Alation Data Catalog              | -                                                                                                                   | Prop            | -           | alation.com                                                 | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Informatica Data Catalog          | -                                                                                                                   | Prop            | -           | informatica.com                                             | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Precisely Data Integrity Suite    | Precisely                                                                                                           | Prop            | -           | precisely.com                                               | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| erwin Data Intelligence           | Quest                                                                                                               | Prop            | -           | quest.com/products/erwin-data-intelligence                  | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| OneTrust Data Discovery           | OneTrust                                                                                                            | Prop            | -           | onetrust.com/products/data-discovery                        | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Collibra Data Catalog             | -                                                                                                                   | Prop            | Github        | collibra.com                                                | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| data.world Data Catalog Platform  | ServiceNow                                                                                                          | Prop            | Github        | data.world                                                  | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Zeenea Data Catalog               | -                                                                                                                   | Prop            | Github        | zeenea.com                                                  | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Explorium                         | -                                                                                                                   | Prop            | Github        | explorium.ai                                                | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Talend                            | -                                                                                                                   | Prop            | -           | talend.com                                                  | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Metaplane                         | -                                                                                                                   | Prop            | -           | metaplane.com                                               | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| BigID Data Intelligence Platform  | -                                                                                                                   | Prop            | -           | bigid.com                                                   | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| IBM watsonx.data intelligence     | -                                                                                                                   | Prop            | -           | ibm.com/products/watsonx-data                               | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Databricks Unity Catalog          | -                                                                                                                   | Cloud           | -           | databricks.com/product/unity-catalog                        | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Snowflake Horizon Catalog         | -                                                                                                                   | Cloud           | -           | snowflake.com/en/data-cloud/horizon                         | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| AWS DataZone                      | -                                                                                                                   | Cloud           | -           | aws.amazon.com/datazone                                     | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Google Cloud Dataplex             | -                                                                                                                   | Cloud           | -           | cloud.google.com/dataplex                                   | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |
| Microsoft Purview                 | -                                                                                                                   | Cloud           | -           | azure.microsoft.com/en-us/products/purview                  | ✔️                                         | ✔️                                     | ✔️                 | ✔️                         | ✔️                                      | ✔️                         | ✔️                     | ✔️                                               | ✔️                                           | ✔️                       | ✔️                      | ✔️               | ✔️            |


### Data Quality, Observability & Governance

Essential features for maintaining data reliability, trustworthiness, observability, collaborative governance, and secure access management. Integral to ensuring metadata-driven AI operations remain accurate, dependable, securely managed, and compliant with sensitive data handling requirements.

## Feature Support Comparison

| Product                   | Vendor / Origin                                                                 | Offering Type | GitHub Repo | Official Website                                            | Data Quality | Data Statistics | Popularity Scoring | Data Status | Collaborative Editing | User Feedback | Sensitive Data Detection | RBAC on Metadata |
|---------------------------|----------------------------------------------------------------------------------|----------------|--------------|--------------------------------------------------------------|--------------|------------------|---------------------|--------------|------------------------|----------------|----------------------------|-------------------|
| Open Data Discovery       | Provectus / Community                                                           | OSS            | [GitHub](https://github.com/opendatadiscovery/odd-platform) | [opendatadiscovery.org](https://opendatadiscovery.org)       | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ❌              | ✔️                         | ✔️                |
| OpenMetadata              | OpenMetadata Community (Collate, ex‑Atlas/Databook)                             | OSS            | [GitHub](https://github.com/open-metadata/OpenMetadata)     | [open-metadata.org](https://open-metadata.org)               | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Amundsen                  | Lyft                                                                            | OSS            | [GitHub](https://github.com/amundsen-io/amundsen)           | [amundsen.io](https://www.amundsen.io)                       | ?            | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         |                   |
| DataHub                   | LinkedIn / DataHub Project                                                      | OSS            | [GitHub](https://github.com/datahub-project/datahub)        | [datahubproject.io](https://datahubproject.io)               | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Marquez                   | WeWork / LF AI & Data                                                           | OSS            | [GitHub](https://github.com/MarquezProject/marquez)         | [marquezproject.ai](https://marquezproject.ai)               | ❌           | ✔️               | ❌                  | ✔️           | ❌                     | ❌             | ❌                         | ✔️                |
| Gravitino                 | Apache Software Foundation                                                      | OSS            | [GitHub](https://github.com/apache/incubator-gravitino)     | [Gravitino](https://incubator.apache.org/projects/gravitino.html) | ❌           | ✔️               | ❌                  | ❌           | ❌                     | ❌             | ❌                         | ✔️                |
| Soda Core                 | Soda                                                                            | OSS            | [GitHub](https://github.com/sodadata/soda-core)             | [soda.io](https://soda.io)                                   | ✔️           | ✔️               | ❌                  | ❌           | ❌                     | ❌             | ✔️                         | ❌                |
| Elementary                | Elementary Data                                                                 | OSS            | [GitHub](https://github.com/elementary-data/elementary)     | [elementary-data.com](https://www.elementary-data.com)       | ✔️           | ✔️               | ❌                  | ❌           | ❌                     | ❌             | ❌                         | ❌                |
| Egeria                    | LF / ODPi                                                                       | OSS            | [GitHub](https://github.com/odpi/egeria)                    | [egeria.odpi.org](https://egeria.odpi.org)                   | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Magda                     | CSIRO / magda.io                                                                | OSS            | [GitHub](https://github.com/magda-io/magda)                 | [magda.io](https://magda.io)                                 | ❌           | ✔️               | ❌                  | ✔️           | ✔️                     | ✔️             | ❌                         | ✔️                |
| Atlas                     | Apache Software Foundation                                                      | OSS            | [GitHub](https://github.com/apache/atlas)                   | [atlas.apache.org](https://atlas.apache.org)                 | ✔️           | ✔️               | ❌                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| CKAN                      | Datopian & Link Digital                                                         | OSS            | [GitHub](https://github.com/ckan/ckan)                      | [ckan.org](https://ckan.org)                                 | ❌           | ❌               | ❌                  | ✔️           | ✔️                     | ✔️             | ❌                         | ✔️                |
| Hamilton                  | Apache Software Foundation                                                      | OSS            | [GitHub](https://github.com/dagworks-inc/hamilton)          | [dagworks.io/hamilton](https://www.dagworks.io/hamilton)     | ✔️           | ✔️               | ❌                  | ❌           | ❌                     | ❌             | ❌                         | ❌                |
| Acryl Data (SaaS DataHub) | -                                                                                  | Prop           | -                  | [acryl.io](https://www.acryl.io)                             | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Collate AI Platform       | Managed OpenMetadata                                                            | Prop           | -                  | [collate.io](https://collate.io)                             | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Atlan                     | -                                                                                  | Prop           | [GitHub](https://github.com/atlanhq/atlan)                  | [atlan.com](https://atlan.com)                               | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Ataccama                  | -                                                                                  | Prop           | -                  | [ataccama.com](https://www.ataccama.com)                     | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Monte Carlo               | -                                                                                  | Prop           | -                  | [montecarlo.com](https://www.montecarlo.com)                 | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Select Star               | -                                                                                  | Prop           | -                  | [selectstar.com](https://www.selectstar.com)                 | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| OvalEdge                  | -                                                                                  | Prop           | -                  | [ovaledge.com](https://www.ovaledge.com)                     | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Datakin                   | -                                                                                  | Prop           | [GitHub](https://github.com/datakin/spline)                 | [datakin.com](https://www.datakin.com)                       | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Alation                   | -                                                                                  | Prop           | -                  | [alation.com](https://www.alation.com)                       | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Informatica               | -                                                                                  | Prop           | -                  | [informatica.com](https://www.informatica.com)               | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Precisely                 | -                                                                                  | Prop           | -                  | [precisely.com](https://www.precisely.com)                   | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| erwin Data Intelligence   | Quest                                                                            | Prop           | -                  | [quest.com](https://www.quest.com/products/erwin-data-intelligence/) | ✔️    | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| OneTrust                  | -                                                                                  | Prop           | -                  | [onetrust.com](https://www.onetrust.com/products/data-discovery) | ✔️        | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Collibra                  | -                                                                                  | Prop           | [GitHub](https://github.com/collibra)                       | [collibra.com](https://www.collibra.com)                     | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| data.world                | ServiceNow                                                                       | Prop           | [GitHub](https://github.com/datadotworld)                   | [data.world](https://data.world)                             | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Zeenea                    | -                                                                                  | Prop           | [GitHub](https://github.com/zeenea)                         | [zeenea.com](https://www.zeenea.com)                         | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Explorium                 | -                                                                                  | Prop           | [GitHub](https://github.com/explorium-ai)                   | [explorium.ai](https://www.explorium.ai)                     | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Talend                    | -                                                                                  | Prop           | -                  | [talend.com](https://www.talend.com)                         | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Metaplane                 | -                                                                                  | Prop           | -                  | [metaplane.com](https://www.metaplane.com)                   | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| BigID                     | -                                                                                  | Prop           | -                  | [bigid.com](https://www.bigid.com)                           | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| IBM watsonx.data          | -                                                                                  | Prop           | -                  | [ibm.com](https://www.ibm.com/products/watsonx-data)         | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Databricks Unity Catalog  | -                                                                                  | Cloud          | -                  | [databricks.com](https://www.databricks.com/product/unity-catalog) | ✔️     | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Snowflake Horizon Catalog | -                                                                                  | Cloud          | -                  | [snowflake.com](https://www.snowflake.com/en/data-cloud/horizon) | ✔️     | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| AWS DataZone              | -                                                                                  | Cloud          | -                  | [aws.amazon.com](https://aws.amazon.com/datazone)           | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Google Cloud Dataplex     | -                                                                                  | Cloud          | -                  | [cloud.google.com](https://cloud.google.com/dataplex)       | ✔️           | ✔️               | ✔️                  | ✔️           | ✔️                     | ✔️             | ✔️                         | ✔️                |
| Microsoft Purview         | -                                                                                  | Cloud          | -                  | [azure.microsoft.com](https://azure.microsoft.com/en-us/products/purview) | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ |


## High-Level Feature Comparison


|                   Tool                    | Specification -Based | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observ- ability | Column-level lineage | Data collaboration |
|:-----------------------------------------:|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:--:|:--:| 
|            [Alation](#alation)            | ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |
|           [Amundsen](#amundsen)           | ❌ | ✔️  | ✔️  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
|           [Ataccama](#ataccama)           | ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |
|              [Atlan](#atlan)              | ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ✔️ | ✔️ |
|              [Atlas](#atlas)              | ❌ | ✔️  | ❌  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
|        [Microsoft Purview](#azure)        | ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ? | ❌ | ❌ | ❌ | ❌ |
|               [CKAN](#ckan)               | ✔️ [DCAT, DCAT-AP, Schema.org and more](https://linkdigital.com.au/news/2024/10/enhancing-dcat-support-in-ckan-dcat-ap-v3-scheming-integration-and-more/) | ✔️ | ❌  | ❌ | ✔️ [details](https://github.com/ckan/ckanext-harvest/)| ❌ | ✔️ [details](https://github.com/ckan/ckanext-qa/) | ❌ | ✔️ [details](https://github.com/ckan/ckanext-archiver/) | ❌ | ❌ |
|           [Collibra](#collibra)           | ❌ | ✔️ | ?  | ✔️ | ❌ | ❌ | ? | ❌ | ❌ | ❌ | ❌ |
|         [DataGalaxy](#datagalaxy)         | ❌ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ❌ | ✔️ | ✔️ | ? | ? |
|           [Databand](#databand)           | ❌ | ? | ? | ? | ❌ | ? | ? | ? | ✔️ | ❌ | ❌ |
|           [Datafold](#datafold)           | ❌ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ |
|            [DataHub](#datahub)            | ✔️ [details](https://datahubproject.io/docs/metadata-modeling/metadata-model/) | ✔️  | ✔️ | ✔️ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
|     [Google Cloud Dataplex](#google)      | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ? | ❌ | ❌ | ❌ | ❌ |
|        [Informatica](#informatica)        | ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ? | ❌ |
|              [Magda](#magda)              | ❌ | ✔️ | ❌  | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
|            [Marquez](#marquez)            | [OpenLineage](https://github.com/OpenLineage/OpenLineage) | ✔️ | ❌| ✔️ | ? | ❌ | ❌ | ❌ | ❌ | ✔️ | ❌ |
|        [Monte Carlo](#montecarlo)         | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ |
|        [Select Star](#selectstar)         | ❌ | ✔️ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ | ✔️ |
| [Open Data Discovery](#opendatadiscovery) | [ODD Specification](https://github.com/opendatadiscovery/opendatadiscovery-specification) | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ❌ | ✔️ |
|       [OpenMetadata](#openmetadata)       | [JSON Schema](https://github.com/json-schema-org/json-schema-spec) | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ |
|             [Stemma](#stemma)             | ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ? | ✔️ | ❌ | ❌ | ❌ |
|             [Talend](#talend)             | ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |
|          [Meta\#Grid](#metagrid)          | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | not yet | ❌ | ❌ | ❌ | ✔️ |
|               [Grai](#grai)               | [Grai Schemas](https://github.com/grai-io/grai-core/tree/master/grai-schemas) | ✔️ | ❌ | ✔️ | ❌ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ✔️ |
|           [Hamilton](#hamilton)           | [Hamilton](https://github.com/dagworks-inc/hamilton) | ✔️ | ✔️ | ? | ✔️ | ❌ | ✔️ | ½ | ✔️ | ✔️ | ❌ |


Definitions:
<ul>
<li><b>Specification-based</b> - uses an open standard for collecting metadata to allow efficient time-to-discovery and federating data catalogs</li>
<li><b>Search-based</b> - allows to search for data assets</li>
<li><b>Network-based</b> - provides rich context about data asset ownership</li>
<li><b>Lineage-based</b> - provides lineage for all entities the solution operates</li> 
<li><b>Federation</b> - the ability to map multiple data catalogs into a single UI to avoid repeated data collection.</li> 
<li><b>ML 1st citizen</b> - operates ML entities on a high level - you can use them as any other data assets.</li> 
<li><b>Data Quality</b> - includes mature data quality assurance tools.</li> 
<li><b>End-to-end lineage</b> - data lineage that includes all data assets used in the organization across all its data catalogs and ML tools.</li> 
<li><b>Column-level lineage</b> - data lineage with column level granularity</li>
<li><b>Data collaboration</b> - provides possibility to bring together data from various internal and external sources to unlock combined data insights</li>
</ul>
<br>

<a name="opensource"></a>
## 📙 Open-Source Data Catalogs

<a name="amundsen"></a>
### Amundsen 
[Website](https://www.amundsen.io/) | [GitHub](https://github.com/amundsen-io/amundsen)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/amundsen-io/amundsen/graphs/commit-activity)
![](https://img.shields.io/github/stars/amundsen-io/amundsen.svg?style=social)

A popular open-source data catalog for metadata management and data discovery originated from Lyft. Created by Amundsen maintainers, [Stemma](stemma.ai) provides a managed version of an enterprise data catalog, inspired by Amundsen.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️  | ✔️  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b>  No</li> 
<li><b>Recommendations:</b> Yes </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> Yes </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> Yes </li>
<li><b>Change notifications:</b>No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> Hive, Redshift, Druid, RDBMS, Presto, Snowflake </li>
</ul>
</details>

<br>

<a name="datahub"></a>
### DataHub

[Website](https://datahubproject.io/) | [GitHub](https://github.com/datahub-project/datahub)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/linkedin/datahub/graphs/commit-activity)
![](https://img.shields.io/github/stars/linkedin/datahub.svg?style=social)

DataHub is an open-source data catalog enabling data discovery, data observability and federated governance that originated from LinkedIn and is commercially offered by Acryl Data as a cloud-hosted SaaS offering.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ✔️ [details](https://datahubproject.io/docs/metadata-modeling/metadata-model/) | ✔️  | ✔️ | ✔️ | ✔ | ✔ | ✔ | ✔ | ❌ | ✔ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push, Pull</li>
<li><b>Customizable metadata model:</b> Yes. The metadata model can be declared using the open-source Pegasus language, and is interoperable with JSONSchema and Avro </li>
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Recommendations:</b> Yes </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> Yes </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> Yes </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> Yes </li>
<li><b>Lineage impact analysis:</b> Yes </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> No </li>
<li><b>Automation:</b> Yes </li>
<li><b>UX personalization:</b> No</li> 
<li><b>Deployment:</b> docker-compose / Kubernetes with Helm, or using Acryl Data's SaaS offering </li> 
<li><b>Supported data sources:</b>
  <ul>
    <li>Snowflake</li>
    <li>BigQuery</li>
    <li>Redshift</li>
    <li>Hive</li>
    <li>Athena</li>
    <li>Postgres</li>
    <li>MySQL</li>
    <li>SQL server</li>
    <li>Trino</li>
    <li>Delta Lake</li>
    <li>S3</li>
    <li>Looker</li>
    <li>PowerBI</li>
    <li>Tableau</li>
    <li>Mode</li>
    <li>Metabase</li>
    <li>Redash</li>
    <li>Superset</li>
    <li>Airflow</li>
    <li>Great Expectation</li>
    <li>dbt</li>
    <li>Feast</li>
    <li>SageMaker</li>
    <li>Glue</li>
    <li>Kafka</li>
    <li>Nifi</li>
    <li>Okta</li>
    <li>LDAP</li>
    <li>Slack</li>
    <li>There's 50+ integrations - see the <a href="https://datahubproject.io/docs/">docs</a> for the latest.</li>
  </ul>
</li>
</ul>
</details>

<br>

<a name="marquez"></a>
### Marquez

[Website](https://marquezproject.github.io/marquez/) | [GitHub](https://github.com/MarquezProject/marquez)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/MarquezProject/marquez/graphs/commit-activity)
![](https://img.shields.io/github/stars/MarquezProject/marquez.svg?style=social)

Marquez is an open-source data catalog for collection, aggregation, and visualization of a data ecosystem’s metadata originated from WeWork. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:-----------:|:--:|:--:|:--:|:---:|:--:|:---:|:--:|:---:|:--:|:---:| 
| [OpenLineage](https://github.com/OpenLineage/OpenLineage) | ✔️ | ❌| ✔️ | ? | ❌ | ❌ | ❌ | ❌ | ✔️ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> S3, Kafka </li>
</ul>
</details>

<br>

<a name="atlas"></a>
### Atlas 

[Website](https://atlas.apache.org/#/) | [GitHub](https://github.com/apache/atlas)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/apache/atlas/graphs/commit-activity)
![](https://img.shields.io/github/stars/apache/atlas.svg?style=social)

Apache Atlas is an open-source data catalog for metadata collection, governance, and data democratization.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️  | ❌  | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> No </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> No</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li>  
<li><b>Supported data sources:</b>HBase, Hive, Sqoop, Kafka, Storm  </li>
</ul>
</details>

<br>

<a name="ckan"></a>
### CKAN

[Website](https://ckan.org/) | [GitHub](https://github.com/ckan/ckan)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/ckan/ckan/graphs/commit-activity)
![](https://img.shields.io/github/stars/ckan/ckan.svg?style=social)

CKAN is an open-source data catalog for data management, widely adopted by governments, NGOs, research institutions, and enterprises. It is actively maintained by a global community, with four of the eight core maintainers currently funded by [Link Digital](https://linkdigital.com.au/).


|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ✔️ Yes (DCAT, DCAT-AP, schema.org via plugins) | ✔️ | ❌  | ❌ | ✔️| ❌ | ✔️ (ckanext-qa) | ❌ | ✔️(ckanext-archiver)| ❌ | ⭕️ (possible via external integrations or Drupal front-end)|

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push, CKAN is used to publish or upload datasets into a central catalog </li>
<li><b>UX personalization:</b> Achievable through integration with CMS platforms like Drupal or any custom front ends. </li> 
<li><b>AI autowiring:</b> Yes. Can be experimented using ckanext-embeddings. </li> 
<li><b>Rich data profiling:</b> Yes, via ckanext-validation extension.</li>
<li><b>Recommendations:</b> Yes. Custom development or integration would be required. </li>
<li><b>Metadata Schemas and Custom Fields:</b> Yes, using ckanext-scheming​.
One of the most widely used extensions for complex metadata schemas.</li>
<li><b>Complex schemas:</b> Yes (via ckanext-dcat extension) </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Visual previews:</b> Yes </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> No </li>
<li><b>Top data users:</b> Achievable using the stats-extension, which provides insights into user activity and dataset popularity.</li>
<li><b>Change notifications:</b> Achievable using ckanext-email-notification. </li>
<li><b>Change feed:</b> Yes </li>
<li><b>Deployment:</b> Yes (Self-hosted, cloud-hosted) </li> 
<li><b>Supported data sources:</b> Yes; various formats:
  <ul>
    <li>Postgres</li>
    <li>MySQL</li>
    <li>SQL server</li>
    <li>PowerBI</li>
    <li>Tableau</li>
    <li>CSV</li>
    <li>Croissant</li>
    <li>JSON</li>
    <li>GeoJSON</li>
    <li>XLS</li>
    <li>Tableau</li>
    <li>...and more!</li>
</ul>
</details>

<br>

<a name="magda"></a>
### Magda

[Website](https://magda.io/) | [GitHub](https://github.com/magda-io/magda)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/magda-io/magda/graphs/commit-activity)
![](https://img.shields.io/github/stars/magda-io/magda.svg?style=social)

Magda is an open-source data catalog that features data discovery, metadata enrichment, and federation, focused on geodata.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️ | ❌  | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push via UI </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> No</li>
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> No </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> ? </li>
<li><b>Change notifications:</b> No </li>
<li><b>Change feed:</b> No </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> Mostly geodata </li>
</ul>
</details>

<br>

<a name="opendatadiscovery"></a>
### Open Data Discovery (ODD) Platform

[Website](https://opendatadiscovery.org/) | [GitHub](https://github.com/opendatadiscovery/odd-platform)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/opendatadiscovery/odd-platform/commits/main)
![](https://img.shields.io/github/stars/opendatadiscovery/odd-platform.svg?style=social)

First open-source data discovery and observability platform. ODD Platform is based on ODD Specification.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ✔️ | ✔️  | ✔️  | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ❌ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push/Pull </li>
<li><b>UX personalization:</b> No </li> 
<li><b>Rich data profiling:</b> Yes </li>
<li><b>Data collaboration:</b> Yes </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> Yes </li>
<li><b>Data preview:</b> No </li>
<li><b>Column statistics:</b> Yes </li>
<li><b>Data owner:</b> Yes </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> Yes </li>
<li><b>Metadata versioning:</b> Yes </li>
<li><b>SaaS:</b> No </li>  
<li><b>Third-party integrations:</b> Airflow, Apache Spark, Dbt, Great Expectations, and Prefect </li>
<li><b>Supported data sources:</b>  Airflow, Athena, AzureSQL, BigQuery, Clickhouse, Databricks, DeltaLake, Druid, DynamoDB, Fivetran, Glue, Hive, Kafka, Looker, MariaDB, MlFlow, MSSQL, MySQL, Oracle, Postgres, Presto, Redash, Redpanda, Redshift, Snowflake, Tableau, and Vertica </li>
</ul>
</details>

<br>

<a name="openmetadata"></a>
### OpenMetadata 

[Website](https://open-metadata.org/) | [GitHub](https://github.com/open-metadata/OpenMetadata)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/open-metadata/OpenMetadata/commits/main)
![](https://img.shields.io/github/stars/open-metadata/OpenMetadata.svg?style=social)

OpenMetadata is the all-in-one platform for data collaboration, discovery, governance, lineage, and quality that lets you focus on building and analyzing.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:|
| ✔️ | ✔️  | ✔️  | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push/Pull </li>
<li><b>UX personalization:</b> No </li> 
<li><b>Rich data profiling:</b> Yes </li>
<li><b>Data collaboration:</b> Yes </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> Yes </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Column statistics:</b> Yes </li>
<li><b>Data owner:</b> Yes </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> Yes </li>
<li><b>Metadata versioning:</b> Yes </li>
<li><b>SaaS:</b> Yes </li>  
<li><b>Third-party integrations:</b> Dbt, Great Expectations, and Prefect </li>
<li><b>Supported data sources:</b> Airbyte, Airflow, Athena, AzureSQL, BigQuery, Clickhouse, Dagster, Databricks, DB2, DeltaLake, Druid, DynamoDB, Fivetran, Glue, Glue, Hive, Kafka, Looker, MariaDB, Metabase, MlFlow, Mode, MSSQL, MySQL, NiFi, Oracle, Postgres, PowerBI, Presto, Redash, Redpanda, Redshift, Salesforce, SingleStore, Snowflake, Superset, Tableau, Trino, and Vertica </li>
</ul>
</details>

<br>

<a name="elementary"></a>
### Elementary

[Website](https://www.elementary-data.com/) | [GitHub](https://github.com/elementary-data/elementary)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/elementary-data/elementary/commits/main)
![](https://img.shields.io/github/stars/elementary-data/elementary.svg?style=social)


<a name="gravitino"></a>
### Apache Gravitino 

[Website](https://gravitino.apache.org/) | [GitHub](https://github.com/apache/gravitino)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/apache/gravitino/commits/main)
![](https://img.shields.io/github/stars/apache/gravitino.svg?style=social)


<a name="soda"></a>
### Soda Core 

[Website](https://www.soda.io/) | [GitHub](https://github.com/sodadata/soda-core)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/sodadata/soda-core/commits/main)
![](https://img.shields.io/github/stars/sodadata/soda-core.svg?style=social)


<a name="metagrid"></a>
### Meta\#Grid 
[Website](https://meta-grid.com/) | [GitHub](https://github.com/patschwork/meta_grid) | [Docs](https://docs.meta-grid.com)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/patschwork/meta_grid/graphs/commit-activity)
![](https://img.shields.io/github/stars/patschwork/meta_grid.svg?style=social)

Meta\#Grid is an open source data catalog for metadata management. It is designed to help small and large organizations create an inventory of their data silos and connect between different technologies. Through a multi-client system, with granular permissions system, Meta\#Grid can be used in consulting companies (with diverse clients and projects) as well as in data mesh organizations. It grows with the requirements of the demand. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | not yet | ❌ | ❌ | ❌ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push, Pull </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b>  No</li> 
<li><b>Recommendations:</b> Yes </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> Yes </li>
<li><b>Data preview:</b> No </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes</li>
<li><b>Top data users:</b> No </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> Yes </li>
<li><b>Deployment:</b>  </li> 
<li><b>Supported data sources:</b> Hive, Redshift, Druid, RDBMS, Presto, Snowflake </li>
</ul>
</details>

<br>


<a name="grai"></a>
### Grai 
[Website](https://grai.io/) | [GitHub](https://github.com/grai-io/grai-core) | [Docs](https://docs.grai.io)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/grai-io/grai-core/graphs/commit-activity)
![](https://img.shields.io/github/stars/grai-io/grai-core.svg?style=social)



|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
| [Grai Schemas](https://github.com/grai-io/grai-core/tree/master/grai-schemas) | ✔️ | ❌ | ✔️ | ❌ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ✔️ |



<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push, Pull</li>
<li><b>Customizable metadata model:</b> Yes. The metadata model can be flexibly extended or modified as needed. </li>
<li><b>Rich data profiling:</b> No </li> 
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes </li>
<li><b>Complex schemas:</b> Yes </li>
<li><b>Data preview:</b> No </li>
<li><b>Column statistics:</b> No </li>
<li><b>Data owner:</b> Yes </li>
<li><b>Top data users:</b> No </li>
<li><b>CI Integration:</b> Yes </li>
<li><b>Lineage impact analysis:</b> Yes </li>
<li><b>Change notifications:</b> Yes </li>
<li><b>Change feed:</b> Yes </li>
<li><b>Automation:</b> Yes </li>
<li><b>UX personalization:</b> Yes </li> 
<li><b>Deployment:</b> docker-compose / Kubernetes with Helm, or using Grai SaaS offering </li> 
<li><b>Supported data sources:</b>
  <ul>
    <li>Snowflake</li>
    <li>BigQuery</li>
    <li>Redshift</li>
    <li>Postgres</li>
    <li>MySQL</li>
    <li>dbt</li>
    <li>Slack</li>
    <li>... many others see the <a href="https://docs.grai.io">docs</a> for a full list.</li>
  </ul>
</li>
</ul>
</details>

<br>

<a name="Hamilton"></a>
### Hamilton 
[GitHub](https://github.com/dagworks-inc/hamilton)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/dagworks-inc/hamilton/commit-activity)
![](https://img.shields.io/github/stars/dagworks-inc/hamilton.svg?style=social)

A popular open-source framework for describing transformations that comes with a catalog (the Hamilton UI). The project originated from Stitch Fix. Created by Hamilton maintainers, [Dagworks Inc. (YCW23)](www.dagworks.io) provides a managed version of the Hamilton UI in addition to self-hosted on-premise features.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:----:|:---:|:---:|:--:|:---:|:--:|:---:|:--:|:---:|:--:| 
[Hamilton](https://github.com/dagworks-inc/hamilton) | ✔️ | ✔️ | ? | ✔️ | ❌ | ✔️ | ½ | ✔️ | ✔️ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Use python to describe DAG, add one-line of code to capture: lineage & provenance, metadata, data summary profiles, versions, and execution telemetry. [See blog for details](https://blog.dagworks.io/p/hamilton-ui-streamlining-metadata). </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Rich data profiling:</b> Pluggable</li> 
<li><b>Recommendations:</b> No </li>
<li><b>Schemas, Description:</b> Yes</li>
<li><b>Complex schemas:</b> Yes </li>
<li><b>Data preview:</b> Only summary statistics </li>
<li><b>Column statistics:</b> Yes, only for python. </li>
<li><b>Data owner:</b> Via tags.</li>
<li><b>Top data users:</b> Not yet </li>
<li><b>Change notifications:</b> Not yet </li>
<li><b>Change feed:</b> No yet</li>
<li><b>Deployment:</b> pip installable locally, self-hosted via docker, managed SaaS </li> 
<li><b>Supported data sources:</b> No direct ingrations as of yet. </li>
</ul>
</details>

<br>

<a name="egeria"></a>
### Egeria 

[Website](https://www.soda.io/) | [GitHub](https://github.com/odpi/egeria)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/odpi/egeria/commits/main)
![](https://img.shields.io/github/stars/odpi/egeria.svg?style=social)



<a name="proprietary"></a>
## 📕 Proprietary Data Catalogs

<a name="collibra"></a>
### Collibra

[Website](https://www.collibra.com) | [GitHub](https://github.com/collibra)

Collibra is an enterprise data catalog that helps to discover and understand data that matters and drive impactful insights from it.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:--:|:---:|:--:|:---:|:-:|:--:|:--:|:--:|:--:|  
| ❌ | ✔️ | ?  | ✔️ | ❌ | ❌ | ? | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="informatica"></a>
### Informatica

[Website](https://www.informatica.com/) | [GitHub](https://github.com/InformaticaCloudApplicationIntegration) 

Informatica is an enterprise data catalog that provides AI-powered data discovery engine to scan and catalog data assets. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:--:|:--:|:---:|:--:|:---:|:--:|  
| ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ? | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> Yes</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

 <br>

<a name="alation"></a>
### Alation

[Website](https://www.alation.com/) | [GitHub](https://github.com/Alation)

Alation is a collaborative data catalog that helps companies to drive value and business impact from their data. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:--:|:--:|:---:|:---:|:---:|:---:|
| ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="atlan"></a>
### Atlan

[Website](https://atlan.com/) | [GitHub](https://github.com/atlanhq)

Atlan is a modern data catalog offering data discovery, data profiling, data quality, data lineage and data governance.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:---:|:---:|:---:| 
| ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ✔️ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b> Presto, Deequ, Atlas, Airflow, Hudi  </li>
</ul>
</details>

<br>

<a name="datagalaxy"></a>
### DataGalaxy

[Website](https://www.datagalaxy.com/en-gb/home/) | [GitHub](https://github.com/datagalaxy-lab)

DataGalaxy is a modern data catalog offering data discovery, data profiling, data quality, data lineage and data governance.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:---:|:---:|:---:| 
| ❌ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ❌ | ✔️ | ✔️ | ? | ? |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull & Push </li>
<li><b>UX personalization:</b> Yes </li> 
<li><b>AI autowiring:</b> Yes</li> 
<li><b>Network-based:</b> Yes</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b> [Available connectors](https://www.datagalaxy.com/fr/integrations-connecteurs/) </li>
</ul>
</details>

<br>

<a name="stemma"></a>
### Stemma

[Website](https://www.stemma.ai/)  

Stemma is a fully managed data catalog powered by the open-source data catalog Amundsen that helps data teams have total trust in their data. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:|
| ❌ | ✔️ | ✔️  | ✔️ | ❌ | ❌ | ? | ✔️ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> No</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="talend"></a>
### Talend

[Website](https://www.talend.com/) | [GitHub](https://github.com/Talend)

Talend is a data catalog that helps enterprises power critical business descisions with trusted data. 

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:| 
| ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>


<a name="selectstar" id="selectstar"></a>
### Select Star

[Website](https://www.selectstar.com/)

Select Star is an intelligent data discovery platform that automatically analyzes and documents your data. Select Star provides an easy to use data portal that everyone can use to find and understand data.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:| 
| ❌ | ✔️ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>AI autowiring:</b> Yes</li>
<li><b>Network-based:</b> Yes</li>
<li><b>Rich data profiling:</b> No</li>
<li><b>ER Diagram generation:</b> Yes</li>
<li><b>Role & Policy based access control:</b> Yes</li>
<li><b>Popularity & usage:</b> Yes </li>
<li><b>Description & Tag propagation:</b> Yes </li>
<li><b>Data preview:</b> Yes </li>
<li><b>Data owners:</b> Yes</li>
<li><b>Top data users:</b> Yes </li>
<li><b>UX personalization:</b> No</li>
<li><b>Supported data sources:</b>
  <ul>
    <li>Snowflake</li>
    <li>BigQuery</li>
    <li>Redshift</li>
    <li>Postgres</li>
    <li>Looker</li>
    <li>PowerBI</li>
    <li>Tableau</li>
    <li>Mode</li>
    <li>Sigma</li>
    <li>Sisense</li>
    <li>Metabase</li>
    <li>Looker Studio</li>
    <li>DBT Cloud & Core</li>
    <li>Slack</li>
  </ul>
</li>
</ul>
</details>

<br>

<a name="monocloud"></a>
## 📒 Monocloud Data Catalogs

<a name="aws"></a>
### Amazon DataZone

[Website](https://aws.amazon.com/datazone/)

Amazon DataZone is a data management service that makes it faster and easier for customers to catalog, discover, share, and govern data stored across AWS, on premises, and third-party sources.

<a name="google"></a>
### Google Cloud Dataplex Universal Catalog

[Website](https://cloud.google.com/dataplex) | [GitHub](https://github.com/GoogleCloudPlatform)

Google Cloud Dataplex Universal Catalog is integrated platform that combines data discovery, cataloging, governance, quality, and exploration into one cohesive service.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:| 
| ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ? | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> No</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="azure"></a>
### Microsoft Purview Unified Catalog

[Website](https://learn.microsoft.com/en-us/purview/)  

Microsoft Purview Unified Catalog is a central platform for discovering, classifying, and managing data assets across organization.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:|
| ❌ | ✔️ | ? | ✔️ | ❌ | ❌ | ? | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>


<a name="databricks"></a>
### Databricks Unity Catalog

[Website](https://www.databricks.com/product/unity-catalog)

<a name="snowflake"></a>
### Snowflake Horizon Catalog

[Website](https://www.snowflake.com/en/product/features/horizon/)

<a name="observability"></a>
## 🔍 Data Observability Platforms

<a name="DataKitchen"></a>
### DataKitchen Open Source Data Observability

[Website](https://docs.datakitchen.io/articles/#!open-source-data-observability/data-observability-overview)  

DataKitchen's Open Source Data Observability Products are full featured with Apache 2.0 license. Data breaks. Servers break. Your toolchain breaks. Ensure your team is the first to know and the first to solve with visibility across and down your data estate. Save time with simple, fast data quality test generation and execution. Trust your data, tools, and systems end to end.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:| 
|  ✔️ | ✔️ |  ✔️ | ✔️ |  ✔️ |  ✔️ | ✔️ |  ✔️ | ✔️ | ❌ | ✔️ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Full featured, with UI for singlue user.  Enterprise version for teams </li>
<li><b>UX personalization:</b> No </li> 
<li><b>AI autowiring:</b> DataOps TestGen data quality verification tool that does five main tasks: (1) data profiling, (2) new dataset screening and hygiene review, (3) AI/algorithmic generation of data quality validation tests, (4) ongoing production testing of new data refreshes and (5) continuous periodic monitoring of datasets for anomalies </li> 
<li><b>Network-based:</b> Data Journey based</li> 
<li><b>Rich data profiling:</b> 51 characteristics, with UI </li> 
<li><b>Supported data sources:</b> Snowflake, Redshift, Tableau, Synapse, Postgres, Tableau, PowerBI, Airflow, Fivetran, Databricks, dbt,  Databricks
Azure Data Factory, SSIS, Synapse Pipelines, ADF-managed Airflow, Google Composer, AWS S3, Qlik Sense, Amazon Managed Workflows for Apache Airflow, Talend Cloud, Azure Functions (via Event Hub), Azure ADLS/Blob Storage (via Event Hub)</li>
</ul>
</details>

<a name="montecarlo"></a>
### Monte Carlo

[Website](https://www.montecarlodata.com/)  

Monte Carlo is a data observability tool that helps to increase trust in data by eliminating or preventing data downtime.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:| 
| ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b> Snowflake, Hive, Kafka, Looker, Redshift, Tableau, Big Query, Airflow, Fivetran, Presto, Mode, Periscope, Databricks, Glue, dbt, Chartio, Spark, AWS, S3, data.world, Google Cloud Platform </li>
</ul>
</details>


<br>

<a name="databand"></a>
### Databand

[Website](https://databand.ai/) | [GitHub](https://github.com/databand-ai/)

Databand is an observability platform that helps data engineers identify and troubleshoot pipeline issues and data quality problems.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:|
| ❌ | ? | ? | ? | ❌ | ? | ? | ? | ✔️ | ? | ? |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a name="datafold"></a>
### Datafold

[Website](https://www.datafold.com/) | [GitHub](https://github.com/datafold)

Datafold is a data monitoring and observability platform that gives you confidence in your data quality through diffs, profiling, and anomaly detection.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:--:|:--:|:--:|:--:|
| ❌ | ✔️ | ✔️ | ✔️ | ❌ | ❌ | ✔️ | ❌ | ✔️ | ? | ? |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Push </li>
<li><b>UX personalization:</b> ?</li> 
<li><b>AI autowiring:</b> ?</li> 
<li><b>Network-based:</b> ?</li> 
<li><b>Rich data profiling:</b> ?</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br> 

<a name="ataccama"></a>
### Ataccama

[Website](https://www.ataccama.com/) | [GitHub](https://github.com/ataccama)

Ataccama is an enterprise data catalog and observability tool featuring data profiling and data quality management, designed for data professionals.

|Based on Open Standard | Search-based | Network-based | Lineage-based | Federation | ML 1st Citizen | Data Quality | End-to-end Lineage | Observability | Column-level lineage | Data collaboration |
|:--:|:---:|:---:|:---:|:--:|:---:|:--:|:---:|:---:|:---:|:---:|
| ❌ | ✔️ | ❌  | ✔️ | ❌ | ❌ | ✔️ | ❌ | ❌ | ❌ | ❌ |

<details>
<summary>More features</summary>
<br>
<ul>
<li><b>Strategy:</b> Pull </li>
<li><b>UX personalization:</b> Yes</li> 
<li><b>AI autowiring:</b> No</li> 
<li><b>Network-based:</b> No</li> 
<li><b>Rich data profiling:</b> Yes</li> 
<li><b>Supported data sources:</b>  </li>
</ul>
</details>

<br>

<a href="#top">Back to top</a>
