# Tanimoto Similarity Search

This script searches KEGG, PubChem, and ChEBI for compounds similar to a given SMILES using Tanimoto similarity.
https://www.ebi.ac.uk/chebi/downloadsForward.do
Download formats
FTP UPDATE:
Most modern browsers (Chrome, Firefox, Safari, etc) have stopped supporting the FTP protocol in the URL's (URL's starting with ftp://). The URL's in this document have been replaced to use HTTPS instead, a protocol that is compatible with modern browsers. However, if you use FTP clients like FileZilla, WinSCP, etc. you are still able to use the FTP URL's to connect.

ChEBI is available from the EBI FTP site. ChEBI can be downloaded in the following formats.

SDF file
ChEBI provides its chemical structures and additional data in SDF format. The data is provided in two flavours,
Chebi_lite_3star.sdf file contains only the chemical structure, ChEBI identifier and ChEBI Name.
ChEBI_complete_3star.sdf file contains all the chemical structures and associated information. Note that it excludes any ontological information as ontological classes are not able to be represented as they do not contain a structure.
More information about the SDF format used in ChEBI can be found in the Developer Manual.
