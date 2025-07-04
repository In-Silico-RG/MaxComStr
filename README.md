# MaxComStr

Here’s the plan for the modular script:

Input a base SMILES: OC(=O)[C@@H]1CC(=C/C=O)C=C(N1)C(=O)O
Search for similar structures in KEGG, PubChem, and ChEBI
Compute Tanimoto similarity

Output a table with:
Structure #
My ID (user-defined)
SMILES
Molecular Formula
Tanimoto Similarity

✅ Key Features:
Modular codebase
Parallelized fetching
Retry logic for failed API requests
Fallbacks for missing data
Unified output to CSV

🧱 Modules:
base_config.py
Stores configuration constants (e.g. thresholds, fingerprints, headers)

fingerprint_utils.py
Handles caching and Tanimoto similarity calculation using RDKit

db_clients/

kegg_client.py – fetch KEGG compounds and structures

pubchem_client.py – search and fetch similar via PubChem

chebi_client.py – search and fetch from ChEBI RDF or web services

main_pipeline.py

Calls all 3 modules
Merges results and removes duplicates
Writes to CSV
Logs failed queries


