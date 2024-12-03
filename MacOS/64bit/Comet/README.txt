2024/10/14

Comet version "2024.02 rev. 0".
https://uwpr.github.io/Comet/releases/release_202402.html

release 2024.02 rev. 0 (2024.02.0), release date 2024/10/14

Add fragment ion indexing support. While fragment ion indexing code was present in the 2024.01 rev. 0 release, this is the first Comet release to official support fragment ion indexing which is a method that was originally implemented by MSFragger. In Comet’s implementation, the fragment ion index is applied as a candidate peptide filter prior to performing full cross-correlation analysis. Please see this page for more details on Comet’s fragment ion index. Thanks to V. Sharma for implementing the modifications permutation code and to E. Bergstrom, C. McGann, and D. Schweppe for driving the development and testing. The following are new search parameters specific to this feature.
fragindex_max_fragmentmass
fragindex_min_fragmentmass
fragindex_min_ions_report
fragindex_min_ions_score
fragindex_num_spectrumpeaks
fragindex_skipreadprecursors
Allow variable modifications to apply to a subset of proteins. For example, one can now limit mono-, di-, and tri-methylation as variable modifications to only histone proteins and not have to apply those modifications on all proteins in the human database. This functionality is controlled by the protein_modlist_file parameter. Note there will be issues for post processing analysis, such as FDR, when applying this feature. Thanks to C. McGann for the feature request.
