---

database-plugin: basic

---
# 001PROJET

```yaml:dbfolder
name: PROJET_CLI
description: PROJET_CLI
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
  installation:
    input: checkbox
    accessorKey: installation
    key: installation
    id: installation
    label: installation start
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
  entreprise_siège:
    input: text
    accessorKey: entreprise_siège
    key: entreprise_siège
    id: entreprise_siège
    label: entreprise_siège
    position: 7
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
    input: select
    accessorKey: entreprise_annexe
    key: entreprise_annexe
    id: entreprise_annexe
    label: entreprise annexe
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 171
    options:
      - { label: "oui", value: "oui", color: "hsl(339, 95%, 90%)"}
      - { label: "non", value: "non", color: "hsl(156, 95%, 90%)"}
      - { label: "oui/non", value: "oui/non", color: "hsl(265, 95%, 90%)"}
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
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 155
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
    input: select
    accessorKey: projet
    key: projet
    id: projet
    label: Type demande
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "3CX", value: "3CX", color: "hsl(317, 95%, 90%)"}
      - { label: "TRUNK", value: "TRUNK", color: "hsl(132, 95%, 90%)"}
      - { label: "Adjonction 3CX", value: "Adjonction 3CX", color: "hsl(239, 95%, 90%)"}
      - { label: "Wifi", value: "Wifi", color: "hsl(35, 95%, 90%)"}
      - { label: "3CX/wifi/Meraki", value: "3CX/wifi/Meraki", color: "hsl(194, 95%, 90%)"}
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
    input: select
    accessorKey: operateur
    key: operateur
    id: operateur
    label: Opérateur_Trunk
    position: 12
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "SFR/Alphalink/UNYC/SEWAN", value: "SFR/Alphalink/UNYC/SEWAN", color: "hsl(45, 95%, 90%)"}
      - { label: "SFR", value: "SFR", color: "hsl(119, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  NbrsTrunk:
    input: number
    accessorKey: NbrsTrunk
    key: NbrsTrunk
    id: NbrsTrunk
    label: NbrsTrunk
    position: 13
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
    input: select
    accessorKey: multisite
    key: multisite
    id: multisite
    label: multisite
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "oui", value: "oui", color: "hsl(223, 95%, 90%)"}
      - { label: "non", value: "non", color: "hsl(315, 95%, 90%)"}
      - { label: "oui_non", value: "oui_non", color: "hsl(319, 95%, 90%)"}
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
    position: 15
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
    input: relation
    accessorKey: matériel
    key: matériel
    id: matériel
    label: matériel
    position: 16
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
      related_note_path: 002DBFLODER/002MATERIEL_CLI/001MATERIEL_CLI.md
      relation_color: hsl(247,70%,39%)
  deadline:
    input: calendar
    accessorKey: deadline
    key: deadline
    id: deadline
    label: deadline
    position: 17
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
    position: 18
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "ETAT/Départ", value: "ETAT/Départ", color: "hsl(354, 95%, 90%)"}
      - { label: "ETAT/Blocage", value: "ETAT/Blocage", color: "hsl(141, 95%, 90%)"}
      - { label: "ETAT/Terminé", value: "ETAT/Terminé", color: "hsl(349, 95%, 90%)"}
      - { label: "INSTALLATION", value: "INSTALLATION", color: "hsl(215, 95%, 90%)"}
      - { label: "#ETAT/En_cours", value: "#ETAT/En_cours", color: "hsl(104, 95%, 90%)"}
      - { label: "#INSTALLATION", value: "#INSTALLATION", color: "hsl(163, 95%, 90%)"}
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
  image:
    input: text
    accessorKey: image
    key: image
    id: image
    label: image
    position: 19
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
    position: 20
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
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 214
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
  SIRET:
    input: text
    accessorKey: SIRET
    key: SIRET
    id: SIRET
    label: SIRET
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
  Date_départ_installation:
    input: calendar
    accessorKey: Date_départ_installation
    key: Date_départ_installation
    id: Date_départ_installation
    label: Date départ installation
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
  Installation_fibre:
    input: select
    accessorKey: Installation_fibre
    key: Installation_fibre
    id: Installation_fibre
    label: Installation fibre
    position: 14
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "SFR", value: "SFR", color: "hsl(340, 95%, 90%)"}
      - { label: "SEWAN", value: "SEWAN", color: "hsl(226, 95%, 90%)"}
      - { label: "UNYC", value: "UNYC", color: "hsl(35, 95%, 90%)"}
      - { label: "ALPHALINK", value: "ALPHALINK", color: "hsl(64, 95%, 90%)"}
      - { label: "N/A", value: "N/A", color: "hsl(52, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  INSTALLATION:
    input: text
    accessorKey: INSTALLATION
    key: INSTALLATION
    id: INSTALLATION
    label: INSTALLATION
    position: 3
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
  row_templates_folder: 002DBFLODER/000PROJET
  current_row_template: 004modèle/MODEL_PROJET.md
  pagination_size: 10
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