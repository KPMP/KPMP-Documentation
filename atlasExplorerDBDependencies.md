# KPMP Explorer UI Database Dependencies

---
# Legend
## Page
### Component (apolloFunctionName -> GraphQLQueryName)
 - associated table
 - associated view
---

## Front Page
### Autocomplete (fetchAutoComplete -> autocomplete) 
 - cell_type
 - cell_type_synonym
 
### Nephron Schematic (fetchCellTypeHierarchy -> cellTypeHierarchy) 
 - cell_type
 - cell_type_synonym
 
## Cell Type Summary (fetchClusterHierarchy -> getClusterHieararchies) 
### Cell Type Summary Table
 - cluster_hierarchy_sp
 
## Diffex
### SNRNASeq Table (fetchGeneExpression -> geneExpressionSummary) 
 - cluster
 - sc_rnaseq
 - sc_cluster_v

### SCRNASeq Table (fetchGeneExpression -> geneExpressionSummary) 
 - cluster
 - sn_rnaseq
 - sn_cluster_v
 
### Regional Transcriptomics Table (fetchRegionalTranscriptomicsByStructure -> getRTGeneExpressionByStructure) 
 - rt_diffex_sp
 
## Gene Summary
### Gene Summary Table (fetchGeneDatasetSummary -> getGeneDatasetInformation)
 - rt_participant_tissue_v
 - participant
 - sc_metadata
 - sc_participant_tissue_v
 - sn_metadata
 - sn_participant_tissue_v
 
## SN/SC Visualization
### Feature Plot (fetchPlotlyData -> getUmapPlotData)
 - sc_feature_data
 - sn_feature_data
 - sc_umap_point_v
 - sn_umap_point_v
 
### Table (fetchGeneExpression -> geneExpressionSummary)
 - sc_cluster_v
 - sc_rnaseq
 - sn_cluster_v
 - sn_rnaseq
 
## RT Visualization
### Plot and Tables (fetchRegionalTranscriptomics -> getRTGeneExpressionByTissue)
#### All Segments
 - rt_segments
 - rt_summary_v
 - segment
 
#### Glom vs. Tub
 - rt_gti
 - rt_summary_v
 - segment
