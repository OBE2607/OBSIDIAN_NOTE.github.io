---
database-plugin: basic
---
# Annuaire

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
    position: 1
    isHidden: false
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
  Entreprise:
    input: text
    accessorKey: Entreprise
    key: Entreprise
    id: Entreprise
    label: Entreprise
    position: 4
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
  Equipe:
    input: tags
    accessorKey: Equipe
    key: Equipe
    id: Equipe
    label: Equipe
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 134
    options:
      - { label: "Chef e projet", value: "Chef e projet", color: "hsl(42, 95%, 90%)"}
      - { label: "Chef de projet", value: "Chef de projet", color: "hsl(231, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Localisation:
    input: tags
    accessorKey: Localisation
    key: Localisation
    id: Localisation
    label: Localisation
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 175
    options:
      - { label: "Beaumont les valence", value: "Beaumont les valence", color: "hsl(276, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Titre:
    input: tags
    accessorKey: Titre
    key: Titre
    id: Titre
    label: Titre
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "#", value: "#", color: "hsl(91, 95%, 90%)"}
      - { label: "Chef de projet", value: "Chef de projet", color: "hsl(81, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  E_MAIL:
    input: text
    accessorKey: E_MAIL
    key: E_MAIL
    id: E_MAIL
    label: E_MAIL
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 244
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_vertical_alignment: align-middle
  Télephone_Fixe:
    input: text
    accessorKey: Télephone_Fixe
    key: Télephone_Fixe
    id: Télephone_Fixe
    label: Télephone Fixe
    position: 9
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
  Télephone_portable:
    input: text
    accessorKey: Télephone_portable
    key: Télephone_portable
    id: Télephone_portable
    label: Télephone portable
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 78
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  NOM:
    input: text
    accessorKey: NOM
    key: NOM
    id: NOM
    label: NOM
    position: 2
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
  Pténom:
    input: text
    accessorKey: Pténom
    key: Pténom
    id: Pténom
    label: Pténom
    position: 3
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
  cover:
    input: text
    accessorKey: cover
    key: cover
    id: cover
    label: cover
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
config:
  remove_field_when_delete_column: false
  cell_size: normal
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
  pagination_size: 10
  font_size: 16
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
```