**cluster_hierarchy_sp (cell_type)**
 - cluster_hierarchy_segments_v

**cluster_hierarchy_by_cluster_sp (cluster)**
 - cluster_hierarchy_segments_v
 
**rt_diffex_sp (structure)**
 - rt_segments
 - cluster_hierarchy_segments_v

**cluster_hierarchy_segments_v**
 - rt_segment_hierarchy_view
 
**sn_sc_rt_shared_clusters_v**
 - rt_segment_hierarchy_v
 - cluster_hierarchy_v
 - abbreviation
 - cell_type 
 
**rt_segment_hierarchy_view**
 - cell_type
 - segment_cell_type_hierarchy_dm
 - segment 

**cluster_hierarchy_v**
 - sn_cluster_hierarchy_v
 - sc_cluster_hierarchy_v
 
**sn_cluster_hierarchy_v**
 - cell_type
 - cluster_celltype
 - cluster
 - sn_metadata
 
**sc_cluster_hierarchy_v**
 - cell_type
 - cluster_celltype
 - cluster
 - sc_metadata
 
---

**umap_point_v**
 - sc_metadata
 - sn_metadata
 - cluster
 
**sn_umap_point_v**
 - sn_metadata
 - cluster
 - participant
 
**sc_umap_point_v**
 - sc_metadata
 - cluster
 - participant
 
---

**sc_cluster_v**
 - sc_metadata
 - cluster
 - participant
 
**sn_cluster_v**
 - sn_metadata
 - cluster
 - participant
 
---

**rt_summary_v (not used?)**
 - rt_summary

---

**rt_participant_tissue_v**
 - participant
 - participant_rt
 
**sc_participant_tissue_v**
 - participant
 - sc_metadata

**sn_participant_tissue_v**
 - participant
 - sn_metadata

 
