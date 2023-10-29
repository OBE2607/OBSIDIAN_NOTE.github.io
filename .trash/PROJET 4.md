---

database-plugin: basic

---
# PROJET

```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 0
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  installation:
    input: checkbox
    accessorKey: installation
    key: installation
    id: installation
    label: installation
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  entreprise_siège:
    input: text
    accessorKey: entreprise_siège
    key: entreprise_siège
    id: entreprise_siège
    label: entreprise_siège
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 110
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  entreprise_annexe:
    input: text
    accessorKey: entreprise_annexe
    key: entreprise_annexe
    id: entreprise_annexe
    label: entreprise annexe
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 171
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  adresse:
    input: text
    accessorKey: adresse
    key: adresse
    id: adresse
    label: adresse
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  projet:
    input: text
    accessorKey: projet
    key: projet
    id: projet
    label: projet
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  operateur:
    input: text
    accessorKey: operateur
    key: operateur
    id: operateur
    label: operateur
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 150
      media_height: 150
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-center
      content_vertical_alignment: align-middle
  NbrsTrunk:
    input: number
    accessorKey: NbrsTrunk
    key: NbrsTrunk
    id: NbrsTrunk
    label: NbrsTrunk
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  multisite:
    input: text
    accessorKey: multisite
    key: multisite
    id: multisite
    label: multisite
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  tech_ref:
    input: text
    accessorKey: tech_ref
    key: tech_ref
    id: tech_ref
    label: tech_ref
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  matériel:
    input: text
    accessorKey: matériel
    key: matériel
    id: matériel
    label: matériel
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  deadline:
    input: calendar
    accessorKey: deadline
    key: deadline
    id: deadline
    label: deadline
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "ETAT/Départ", value: "ETAT/Départ", color: "hsl(305, 95%, 90%)"}
      - { label: "ETAT/En_cours", value: "ETAT/En_cours", color: "hsl(73, 95%, 90%)"}
      - { label: "ETAT/Blocage", value: "ETAT/Blocage", color: "hsl(341, 95%, 90%)"}
      - { label: "ETAT/Terminé", value: "ETAT/Terminé", color: "hsl(25, 95%, 90%)"}
      - { label: "INSTALLATION", value: "INSTALLATION", color: "hsl(12, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  image:
    input: text
    accessorKey: image
    key: image
    id: image
    label: image
    position: 100
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  cover:
    input: text
    accessorKey: cover
    key: cover
    id: cover
    label: cover
    position: 100
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  CANEVA:
    input: text
    accessorKey: CANEVA
    key: CANEVA
    id: canva
    label: canva
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-center
      content_vertical_alignment: align-middle
config:
  remove_field_when_delete_column: false
  cell_size: wide
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 25
  font_size: 10
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: dd-MM-yyyy
  datetime_format: "dd-MM-yyyy HH:mm:ss"
  metadata_date_format: "dd-MM-yyyy HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
      - field: entreprise_siège
        operator: CONTAINS
        value: "non_entreprise"
        type: text
      - condition: AND
        disabled: false
        label: "firme"
        color: "hsl(244,100%,50%)"
        filters:
        - field: adresse
          operator: CONTAINS
          value: ""
          type: text
```