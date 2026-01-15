# biograph_chatgpt
Biomedical Knowledge Graph

This project provides a turnkey framework for building and serving a rich knowledge graph across life‑science and corporate domains.  It combines authoritative public data (clinical trials, pathway and ontology databases, patents and filings, news and legal entity registries) with a simple schema and a set of ingestion scripts.  The goal is to create a structured, queryable representation of drugs, diseases, genes/proteins, companies and their interactions, backed by a Postgres database and exposed via a REST API.

Features

	•	Open data ingestion – Load free, royalty‑free datasets such as MeSH, Gene Ontology, ClinicalTrials.gov, OpenFDA, Open Targets, USPTO patents, SEC filings and GLEIF LEI data.  Each loader script downloads and normalises the source into the shared schema.

	•	Extendable schema – A minimal SQL schema defines entity, alias and edge tables for core graph elements, plus supporting tables for MeSH descriptors and clinical trials.  Additional ontologies or sources can be mapped into these tables or new tables added as needed.

	•	FastAPI service – A lightweight API exposes endpoints to check health, seed demo data, and list entities and edges.  It can be extended with additional endpoints for search, analytics or graph algorithms.

	•	Turnkey setup – Deploy locally using Postgres (e.g. [Neon free tier] or Docker), run the loader scripts to ingest data, then start the API.  Scripts are dependency‑light and do not require commercial licences.

	•	Pluggable entity resolution – The design anticipates a modern entity‑resolution pipeline using embeddings and graph neural networks; you can integrate such a pipeline to deduplicate and link entities across datasets.

Repository structureBiomedical Knowledge Graph

This project provides a turnkey framework for building and serving a rich knowledge graph across life‑science and corporate domains.  It combines authoritative public data (clinical trials, pathway and ontology databases, patents and filings, news and legal entity registries) with a simple schema and a set of ingestion scripts.  The goal is to create a structured, queryable representation of drugs, diseases, genes/proteins, companies and their interactions, backed by a Postgres database and exposed via a REST API.

Features

	•	Open data ingestion – Load free, royalty‑free datasets such as MeSH, Gene Ontology, ClinicalTrials.gov, OpenFDA, Open Targets, USPTO patents, SEC filings and GLEIF LEI data.  Each loader script downloads and normalises the source into the shared schema.

	•	Extendable schema – A minimal SQL schema defines entity, alias and edge tables for core graph elements, plus supporting tables for MeSH descriptors and clinical trials.  Additional ontologies or sources can be mapped into these tables or new tables added as needed.

	•	FastAPI service – A lightweight API exposes endpoints to check health, seed demo data, and list entities and edges.  It can be extended with additional endpoints for search, analytics or graph algorithms.

	•	Turnkey setup – Deploy locally using Postgres (e.g. [Neon free tier] or Docker), run the loader scripts to ingest data, then start the API.  Scripts are dependency‑light and do not require commercial licences.

	•	Pluggable entity resolution – The design anticipates a modern entity‑resolution pipeline using embeddings and graph neural networks; you can integrate such a pipeline to deduplicate and link entities across datasets.
