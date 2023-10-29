
# 02 - 04 - Plugin-Multi-Column Markdown

>[!note]+ lien
>https://efemkay.github.io/obsidian-modular-css-layout/multi-column/02-multi-column-callout/

Multi-Column Markdown

Prenez votre document de démarquage ennuyeux et ajoutez-y des colonnes ! Avec Multi Column Markdown plutôt que de limiter la mise en page de votre document à un seul fichier linéaire, vous pouvez désormais définir des blocs de données à disposer horizontalement les uns à côté des autres. Cette fonctionnalité supplémentaire vous donne la liberté de structurer vos notes de manière plus créative.


Core Features

- Define customizable column layouts within your Obsidian documents.
- Setup your columns to look how you want, being able to define number of columns, widths, spacing, text alignment and more.
- Muliple syntax options including Pandoc compatible [fenced divs](https://github.com/dialoa/columns/blob/master/README.md).
- Setup entire documents to automatically reflow into multiple columns when viewed in Obsidian's reading mode.

Table of Contents

- [Usage](https://github.com/ckRobinson/multi-column-markdown#usage)
- [Syntax Reference](https://github.com/ckRobinson/multi-column-markdown#syntax-reference)
- [Region Settings](https://github.com/ckRobinson/multi-column-markdown#region-settings)
- [Multi-Column Reflow](https://github.com/ckRobinson/multi-column-markdown#full-document-multi-column-reflow)
- [Available Commands](https://github.com/ckRobinson/multi-column-markdown#plugin-commands)
- [Installation](https://github.com/ckRobinson/multi-column-markdown#installation)
- [Known Issues](https://github.com/ckRobinson/multi-column-markdown#known-issues)
- [Change Log](https://github.com/ckRobinson/multi-column-markdown#change-log)

A Word On Live Preview

Live preivew has been supported in Multi-Column Markdown, however cross compatibilty with other plugins, anything that requires interaction (IE: button clicks), and more advanced, non-naitive markdown, Obsidian features may or may not be supported in this mode.

Due to how custom live preview plugins are implemented within CodeMirror6 and hook into Obsidian, I can not guarentee all plugins will render properly within live preview at this point. Plugins that do not render their content immediatly, such as needing to wait for a dataview query, do not render properly.

This plugin was originally intended for use only in Reading mode where plugins have more control over how content is rendered. Most plugins, interactive elements, advanced markdown, and visual stylings will render better and have more cross compatibility in Reading mode.

Usage:

You create a multi-column region by defining the start, settings, column-end, and end tags. EG:

Text displayed above.

```start-multi-column

ID: ExampleRegion1

number of columns: 2

largest column: left

```

Text displayed in column 1.

--- end-column ---

Text displayed in column 2.

--- end-multi-column

Text displayed below.

Rendered as:

[![Example_1](

Syntax Reference

Region Start Tag:

Each multi-column region must start with either:

```start-multi-column

ID: A_unique_region_ID

```

or

```multi-column-start

ID: A_unique_region_ID_1

```

or

::::: {.columns id=A_unique_region_ID_2}

(See more about Pandoc's fenced divs syntax below.)

After defining the start tag you must declare an ID for the region. The ID is used to differentiate between different regions if there are multiple in the same document.

Each ID must be unique within the same document or unexpected render issues may occur. An ID may be used across multiple documents so that, for example, you can use the ID "dailynote" in the template used for your Periodic Notes.

By using the "Insert Multi-Column Region" command (more below) the start ID will be pre-set as a randomly generated 4 character string.

You can also use the "Fix Missing IDs" command which will search the currently open document and append random IDs to all regions that are missing one.

Valid Syntax Tags:

Each tag type can be defined with the following options:

Start Multi-Column Region:

```start-multi-column

ID: A_unique_region_ID

Any Additional Setting flags (see below)

```

```multi-column-start

ID: A_unique_region_ID_2

Any Additional Setting flags (see below)

```

::::: {.columns id=A_unique_region_ID_2 Any Additional Setting flags (see below)}

End a Column:

--- column-end ---

--- end-column ---

--- column-break ---

--- break-column ---\

::: columnbreak

:::

(New line after columnbreak required.)

End Multi-Column Region:

--- end-multi-column

--- multi-column-end\

:::

(This end region syntax is only valid when using the Pandoc fenced divs syntax to start a region.)

Pandoc Fenced Divs Support

You can also use Pandoc's fenced divs syntax to define column regions. (For more detail on this syntax see [here](https://pandoc.org/MANUAL.html#divs-and-spans) and [here](https://github.com/dialoa/columns/blob/master/README.md).)

To create a multicolumn region use:

::: columns

<Column Content>

:::

To define multiple Pandoc regions on the same document, and to define region settings you must use the attributes syntax:

::::: {.columns property=value id=ID_ExampleID}

<Column Content>

:::::

Not providing an ID will cause regions to not render.

All other settings can be defined within the attributes using the same setting flag names defined below.

What is supported with this syntax:

- Basic fenced divs column definition: '::: columns' or '::: {.columns}'
- Specifying the number of columns with english words up to ten: '::: twocolumns', '::: {.three-columns}', etc.
- Specifying the number of columns through attributes: '::: {.columns col-count=3}'
- Specifying column gap through attributes: '::: {.columns columngap=3em}'
- Specifying column breaks through column break div: :::: columnbreak\n::::

What is not supported:

- Recusive Column Regions. Recusive regions are not supported in Core MCM so will not render the same as an exported Pandoc PDF.
- Spanning element. Elements that break up a column region to span across the view are not supported. You must manually end the region and start a new one.
- Specifying 'column rule', as there is currently no way to define this with other syntax.
- Justified or ragged column mode.
- "Fluid Columns" by default. The fluid columns default of Pandoc's syntax is equivalent to MCM's Auto Layout. However auto layout has significant perforamce overhead in Live preview and due to this Pandoc syntax will not automatically flag regions to auto layout. You can however manually flag them by adding the setting to the attributes: ::: {.three-columns fluid-columns=true} or ::: {.three-columns auto-layout=true}

Region Settings:

ID:

- Setting Flags:

- ID:

- Valid Selections:

- Any string of characters.

Example:

```start-multi-column

ID: Random_ID_String

```

- The ID is used to differentiate between different regions if there are multiple in the same document.
- Each ID must be unique within the same document or unexpected render issues may occur. An ID may be used across multiple documents so that, for example, you can use the ID "dailynote" in the template used for your Periodic Notes.
- Can be ommitted if there will only ever be a single column region in the document.

Number of Columns:

- Setting Flags:

- Number of Columns:
- Num of Cols:
- Col Count:

- Valid Selections:

- Any digit.

Example:

```start-multi-column

Number of Columns: 2

```

Column Size:

By default all of the columns will be set to equal size if this option is omitted.

Can define on a per column basis with array syntax: EG: [25%, 75%]

- Setting Flags:

- Column Size:
- Col Size:
- Column Width:
- Col Width:
- Largest Column:

- Valid Selections:

- Single Column layout:

- Small
- Medium
- Large
- Full

- For either 2 or 3 column layouts

- Standard
- Left
- First
- Right
- Second

- Only for 3 column layouts

- Center
- Third
- Middle

- Allows most CSS unit lengths (px, pt, %, etc).

Example:

```start-multi-column

Column Size: standard

( OR )

Column Size: [25%, 75%]

```

Border:

By default the border is enabled but can be removed with:

Can define on a per column basis with array syntax: EG: [off, on, off]

- Setting Flags:

- Border:

- Valid Selections:

- disabled
- off
- false

Example:

```start-multi-column

Border: disabled

( OR )

Border: [off, on]

```

Shadow:

On by default, can be removed with:

- Setting Flags:

- Shadow:

- Valid Selections:

- disabled
- off
- false

Example:

```start-multi-column

Shadow: off

```

Column Position or Column Location:

Only used with the single column option.

- Setting Flags:

- Column Position:
- Col Position:
- Column Location:
- Col Location:

- Valid Selections:

- Left
- Right
- Center
- Middle

Example:

```start-multi-column

Number of Columns: 1

Column Position: Left

```

Column Spacing:

Used to set the distance between all of the columns.

Can define on a per column basis with array syntax: EG: [5px, 10px]

- Setting Flags:

- Column Spacing:

- Valid Selections:

- Allows most CSS unit lengths (px, pt, %, etc).
- A number alone without a defined unit type defaults to pt unit.

Example:

```start-multi-column

Column Spacing: 5px

( OR )

Column Spacing: [5px, 10px]

```

Content Overflow:

Should the columns cut off anything that goes outside the column bounds or should it be scrollable.

Can define on a per column basis with array syntax: EG: [Scroll, Hidden]

- Setting Flags:

- Overflow:
- Content Overflow:

- Valid Selections:

- Scroll (Default)
- Hidden

Example:

```start-multi-column

Overflow: Hidden

( OR )

Overflow: [Scroll, Hidden]

```

Alignment:

Choose the alignment of the content in the columns.

Can define on a per column basis with array syntax: EG: [Left, Center]

- Setting Flags:

- Alignment:
- Content Alignment:
- Content align:
- Text Align:

- Valid Selections:

- Left (Default)
- Center
- Right

Example:

```start-multi-column

Alignment: Center

( OR )

Alignment: [Left, Center]

```

Auto Layout

- Setting Flags:

- Auto Layout:
- Fluid Columns:
- Fluid Cols:

- Valid Selections:

- true
- on

Example:

```start-multi-column

Auto Layout: on

```

---

Auto layout regions do not use defined column breaks. Instead these type of multi-column regions will attempt to balance all content equally between the columns. Headings are also attempted to be preserved so that a heading block will not end a column but will instead be moved to the top of the next column with it's corresponding content.

To use this feature set "Auto Layout: true" within the region settings.

Full Document Multi-Column Reflow

Documents can be set to fully reflow into multiple columns while in Reading mode.

Syntax

To enable document reflow use Obsdian's frontmatter to provide the metadata for the file with the following syntax:

EG:

---  
Multi-Column Markdown:  
  - Number of columns: 3  
  - Alignment: [Left, Center, Left]  
  - Border: off  
---

First line of document.

All settings must be a list underneath the Multi-Column Markdown tag. If obsidian does not parse a valid syntax it will not render. You can use the "Setup Multi-Column Reflow" command to ensure proper syntax.

Features:

- Reflow automatically detects your document view size and sets the column heights to match, reducing the number of times you need to scroll through the document.

- Auto column height is overridable by defining the col-height in frontmatter settings using standard MCM syntax.
- Changes to the view size currently require a document reload to update layout.

- User definable column breaks using default Multi-Column Markdown column break syntax.

Additional Notes:

- Just as with core MCM, the default Obsidian theme, all basic markdown syntax and rendered elements should be fully supported. However cross compatibility with other plugins, embeds, and themes are not guarenteed.
- All manually set multi-column regions are overridden by the document reflow.

Known Issues:

- Changes to the document may require a file reload to properly update.
- Export to PDF is currently not supported.
- Long paragraphs of text will not be split across columns, as they are rendered as a single chunks of content by Obsidian.

Plugin Cross Compatibility.

Not all plugins will be cross compatable within a multi-column region. Depending on the implementation or use case, some plugins will either entierly not render, render incorrectly, or render but be uninteractable. For the most part, due to how Obsidian plugins work, there is little that can be done at this stage to guarentee cross compatibility. And this is even more the case when using Live Preview. You can check the [Cross Compatibility](https://github.com/ckRobinson/multi-column-markdown/blob/master/documentation/CrossCompatibility.md) sheet for plugins known to work within columns. Anything not on that list has not been tested.

Obsidian Theming

Just as with cross compatibilty above, multi-column regions may be effected by the Obsidian Theme you are running. There is very little non-layout dependent CSS within MCM but some themes may add or remove elements neccessary to properly render the columns. If regions do not render properly in a specific theme, feel free to open an issue and make sure to include what Obsidian theme you are running when describing the problem.

Full Mutli-Column Examples:

[Here](https://github.com/ckRobinson/multi-column-markdown/blob/master/documentation/FullExamples.md)

Plugin Commands:

You can access the command pallet with ctrl/command - P.

Insert Multi-Column Region

Will create a two column region where the cursor is located with a randomly generated ID and a default settings block created. Anything currently selected will be moved outside the end of the inserted region as to not overwrite any data.

Fix Missing IDs For Multi-Column Regions

Will search the current document for any region start tags that are missing IDs and randomly generate new IDs for each region.

Toggle Mobile Rendering - Multi-Column Markdown

Enables or disables column rendering on mobile devices only.

Setup Multi-Column Reflow

Adds the default multi-column reflow tags and settings to the document frontmatter. Will not overwrite if already defined.

Installation

From Obsidian Community Plugins

You can install this plugin from the Obsidian Community Plugins menu by following these steps:

- Open Settings within Obsidian
- Click Community plugins and ensure Safe mode is disabled
- Browse community plugins and find "Multi-Column Markdown"
- Click Install
- After installation is finished, click Enable

From GitHub Repository

Download main.js, manifest.json, styles.css from the latest release and add a new directory: [Obsidian-vault]/.obsidian/plugins/multi-column-markdown and add the files to that directory.

If this is your first Obsidian plugin close and reopen Obsidian and then open the settings menu, click the Community plugins tab to the left, ensure Safe mode is disabled, and then enable "Multi-Column Markdown" in the installed plugins list.

Known Issues

Live Preview

- Any file interaction causes embeds to reload.

- All issues of this kind are due to Obsidian redrawing the entire editor on every file interaction (click, keystroke, etc). The redraw causes all embeds to be re-loaded which makes them appear to flash on screen. There is currently no solution to this problem.

- Some cross compatibility with other plugins is not supported and will not render.

- Most plugins that do not render are more advanced plugins that load their content over time rather than immediatly at render time.

- Clicking within a document causes the document to flash before recentering on the cursor location.
- Clicking outside of the editor and then back in may cause the viewport to jump to the bottom of the editor in certain circumstances.

Codeblock Start Tags

- Having an edit view and reading view of the same document open at the same time causes render issues when using codeblock start tags.

Minor Render Issues

- Any general render issues within columns:

- If columns render their content in an unexpected way try swapping to a new file and back, this will usually fix the issue.

- When entering data into a multi-column region the data can sometimes be rendered a line above or below the intended location in the preview window. When the line is near the start or end of a column or region it may be rendered in the wrong column or outside of the region entirely.
- Copy and pasting text into a new locations within a region may not update in preview view properly.
- When swapping between auto layout or single column, regions may sometimes become stuck rendering an old layout.
- Auto layout regions sometimes get stuck in a non-equal state.

- Workaround:

- Swapping to a different file and back, or closing and reopeing the file will force a reload of the data and fix the render issue.

Other

- Exporting a document with pandoc columns that contains other embedded fenced divs will not export properly.
- Changes to a document may require a file reload to properly update Multi-Column Reflow.
- Long paragraphs of text will not be split across columns in Multi-Column Reflow, as they are rendered as a single chunks of content by Obsidian.
- The Obsidian API and this plugin are both still works in progress and both are subject to change.

Depreciated

These syntax options are currently still supported but are being depreciated for the newer syntax above.

Start Multi-Column Region:

- === start-multi-column: A_unique_region_ID_2
- === multi-column-start: A_unique_region_ID_3

Settings Regions:

```settings```

```column-settings```

```multi-column-settings```

End a Column:

- === column-end ===
- === end-column ===
- === column-break ===
- === break-column ===

End Multi-Column Region:

- === end-multi-column
- === multi-column-end

Change Log

0.8.3

- Fixed issue when button plugin directly embeded into column region, causing button to not render.

0.8.2

- Fixed issue with button plugin cross compatibility, causing buttons to sometimes not render and be uninteractable.

0.8.1

- Minor Changes

- Updated viewport re-focusing to fix scrolling to end of document when selecting text.
- Updated viewport re-focus to reduce unnecessary updates.
- Updated image rendering to hopefully solve images not rendering in Reading Mode.
- Updated to include webp images in live preview rendering.
- Overhauled portion of element rendering in preparation for larger rework.

0.8.0

- Unlimited Columns

- You can now define an unlimited number of columns within your settings blocks. All columns that extend beyond the viewport will be visible when scrolling the column region.
- Use the column size settings flag and the new settings array syntax to define custom column widths.  
    (EG: "Column size: [20%, 30%, 50%, 100%]")
- Implemented for FR #45, #46, #47

- Multiple setting values per column

- You can now define certain settings to be different for each column.
- Use the syntax: "Alignment: [Left, Center, Right]"
- The following settings can be defined in this way:

- Column Size
- Column Border
- Column Spacing
- Column Overflow
- Text Alignment

- Live preview scroll "fix"

- Added new CM6 module that attempts to alleviate the viewport scroll issue in live preview.
- The module attempts to keep the viewport centered on the cursor by moving the view after Obsidian re-renders the document.
- Known issues:

- The viewport will appear to flash as it jumps to the new cursor location. This appears to be more or less noticable depending on the machine.
- Swapping out and back into Obsidian causes the document to jump to the bottom of the document.
- Clicking back into an editor view without moving the cursor can cause the viewport to jump to the bottom of the document.

- Pandoc Multi-Column Syntax

- Added support for the fenced dives syntax used with Pandoc per FR #71.
- Not all of the fenced divs syntax is currently supported.
- If you use multiple regions on the same document you must also include an ID within the attributes: ::: {columns id=A_unique_region_ID_4}
- What is supported:

- Basic fenced divs column definition: ::: columns or ::: {.columns}
- Specifying the number of columns through english up to ten: ::: twocolumns, ::: {.three-columns}, etc.
- Specifying the number of columns through attributes: ::: {.columns col-count=3}
- Specifying column gap through attributes: ::: {.columns columngap=3em}
- Specifying column breaks through column break div: :::: columnbreak\n::::

- What is not supported:

- Recusive Column Regions. Recusive regions are currently not supported in Core MCM so will not render the same as an exported Pandoc PDF.
- Spanning element. Elements that break up a column region to span across the view are not supported. You must manually end the region and start a new one.
- Specifying column rule, as there is currently no way to define this with other syntax. Will hopefully be added in the future.
- Justified or ragged column mode.
- "Fluid Columns" by default. The fluid columns default of Pandoc's syntax is equivalent to MCM's Auto Layout. However auto layout has significant perforamce overhead in Live preview and due to this Pandoc syntax will not automatically flag regions to auto layout. You can however manually flag them by adding the setting to the attributes: ::: {.three-columns fluid-columns=true} or ::: {.three-columns auto-layout=true}

- Known Issues:

- Exporting a document with pandoc columns that contains other embedded fenced divs will not export properly.

- Full Document Multi-Column Reflow

- Documents can now be set to fully reflow into multiple columns. Per FR #70
- The multi-column reflow is only visible while in Reading mode.
- Features:

- Use core Obsidian yaml frontmatter to define what documents should reflow.
- Reflow automatically detects your document view size and sets the column heights to match, reducing the number of times you need to scroll through the document.

- Auto column height is overridable by defining the col-height in frontmatter settings using standard MCM syntax.
- Changes to the view size currently require a document reload to update layout.

- User definable render settings from within the frontmatter. (See example below.)

- You must use valid Obsidian frontmatter syntax to define the settings or they will not be applied.

- User definable column breaks using default Multi-Column Markdown column break syntax.
- 'Setup Multi-Column Reflow' command will assist in setting proper yaml syntax to Obsidian frontmatter.

- Additional Notes:

- Just as with core MCM, the default Obsidian theme, all basic markdown syntax and rendered elements should be fully supported. However cross compatibility with other plugins, embeds, and themes are not guarenteed.
- All manually set multi-column regions are overridden by the full document reflow.

- Known Issues:

- Changes to the document may require a file reload to properly update.
- Export to PDF is currently not supported.
- Long paragraphs of text will not be split across columns, as they are rendered as a single chunks of content by Obsidian.

Syntax Example:

---  
Multi-Column Markdown:  
  - Number of columns: 3  
  - Alignment: [Left, Center, Left]  
  - Border: off  
---

[Full Example Here](https://github.com/ckRobinson/multi-column-markdown/blob/master/documentation/FullExamples.md#multi-column-reflow)

- Minor Changes

- Updated column break flag to trigger properly when attached to the end of lists.
- Added new check for custom frame plugins that fixes rendering in view mode.
- Fixed a bug that caused theme CSS to not apply to tables when rendered in live preview.
- Updated live preview to properly render PDFs.
- Attempted to fix cross compatibilty with "Buttons" plugin in Reading mode. #72
- Added error message when user embeds a file within a live preview region.

Older Changes:

[Change log](https://github.com/ckRobinson/multi-column-markdown/blob/master/ChangeLog.md)

Support Me:

[![Buy Me A Coffee](data:image/png;base64,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)](https://www.buymeacoffee.com/ckrobinson)

[![Buy Me a Coffee at ko-fi.com](data:image/png;base64,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)](https://ko-fi.com/ckrobinson)

About

A plugin for the Obsidian markdown note application, adding functionality to render markdown documents with multiple columns of text.

Resources

[Readme](https://github.com/ckRobinson/multi-column-markdown#readme)

License

[GPL-3.0 license](https://github.com/ckRobinson/multi-column-markdown/blob/master/LICENSE)

[Activity](https://github.com/ckRobinson/multi-column-markdown/activity)

Stars

[151 stars](https://github.com/ckRobinson/multi-column-markdown/stargazers)

Watchers

[4 watching](https://github.com/ckRobinson/multi-column-markdown/watchers)

Forks

[7 forks](https://github.com/ckRobinson/multi-column-markdown/forks)

[Report repository](https://github.com/contact/report-content?content_url=https%3A%2F%2Fgithub.com%2FckRobinson%2Fmulti-column-markdown&report=ckRobinson+%28user%29)

[Releases 25](https://github.com/ckRobinson/multi-column-markdown/releases)

[0.8.3 Latest](https://github.com/ckRobinson/multi-column-markdown/releases/tag/0.8.3)

[Jun 26, 2023](https://github.com/ckRobinson/multi-column-markdown/releases/tag/0.8.3)

[+ 24 releases](https://github.com/ckRobinson/multi-column-markdown/releases)

[Packages](https://github.com/users/ckRobinson/packages?repo_name=multi-column-markdown)

No packages published

Languages

- [TypeScript98.1%](https://github.com/ckRobinson/multi-column-markdown/search?l=typescript)
- [CSS1.3%](https://github.com/ckRobinson/multi-column-markdown/search?l=css)

- [JavaScript0.6%](https://github.com/ckRobinson/multi-column-markdown/search?l=javascript)

Footer

 © 2023 GitHub, Inc.

Footer navigation

- [Terms](https://docs.github.com/site-policy/github-terms/github-terms-of-service)
- [Privacy](https://docs.github.com/site-policy/privacy-policies/github-privacy-statement)
- [Security](https://github.com/security)
- [Status](https://www.githubstatus.com/)
- [Docs](https://docs.github.com)
- [Contact GitHub](https://support.github.com?tags=dotcom-footer)
- [Pricing](https://github.com/pricing)
- [API](https://docs.github.com)
- [Training](https://services.github.com)
- [Blog](https://github.blog)
- [About](https://github.com/about)

À partir de l’adresse <[https://github.com/ckRobinson/multi-column-markdown](https://github.com/ckRobinson/multi-column-markdown)>