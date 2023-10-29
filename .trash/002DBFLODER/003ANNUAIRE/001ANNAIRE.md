---

database-plugin: basic

---
# 001ANNAIRE

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
      content_alignment: text-align-center
      content_vertical_alignment: align-middle
  nom:
    input: text
    accessorKey: nom
    key: nom
    id: nom
    label: nom
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
  Type:
    input: text
    accessorKey: Type
    key: Type
    id: Type
    label: Type
    position: 2
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
  Prénom:
    input: text
    accessorKey: Prénom
    key: Prénom
    id: Prénom
    label: Prénom
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
  Entreprise:
    input: text
    accessorKey: Entreprise
    key: Entreprise
    id: Entreprise
    label: Entreprise
    position: 5
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
  Projet:
    input: relation
    accessorKey: Projet
    key: Projet
    id: Projet
    label: Projet
    position: 6
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
      related_note_path: 002DBFLODER/000PROJET/PROJET.md
      relation_color: hsl(192,36%,42%)
  Localisation:
    input: text
    accessorKey: Localisation
    key: Localisation
    id: Localisation
    label: Localisation
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 195
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Email:
    input: text
    accessorKey: Email
    key: Email
    id: Email
    label: Email
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 248
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  TELFixe:
    input: text
    accessorKey: TELFixe
    key: TELFixe
    id: TELFixe
    label: Téléphone fixe
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 120
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
      wrap_content: true
  TELPort:
    input: text
    accessorKey: TELPort
    key: TELPort
    id: TELPort
    label: Téléphone portable
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 127
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
      content_vertical_alignment: align-middle
      content_alignment: text-align-center
  image:
    input: text
    accessorKey: image
    key: image
    id: image
    label: image
    position: 11
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
    position: 12
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
  Selection:
    input: select
    accessorKey: Selection
    key: Selection
    id: tags
    label: Type de contact
    position: 13
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "CDP", value: "CDP", color: "hsl(304, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
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
  row_templates_folder: 002DBFLODER/003ANNUAIRE/000ANNUAIRE
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