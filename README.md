# Blender API

[**WEB**](https://tomashubelbauer.github.io/blender-api)

Interesting methods from the Blender API I figured to make a note of.

## Context Access (`bpy.context`)

- `area` - viewport dimensions and the view mode
- `blend_data` - parsed Blend file
- `collection` - all objects in the scene?
- `engine` - engine ID like `CYCLES` and `BLENDER_EEVEE`?
- `gizmo_group` - gizmos are the rotating things in the viewport, no?
- `layer_collection` - this I think replaces the former 20 hardcoded layers
- `mode` - viewport mode
- `preferences` - access to user settings
- `region` - how does this differ from `area`?
- `region_data` - ?
- `scene`
- `screen` - editor settings?
- `space_data` - how is this different from screen, region and area?
- `tool_settings` - various thresholds and values for tools
- `view_layer` - calling update on it recalculates texts
- `window` - allows moving and setting the cursor and faking keyboard input
- `window_manager` - access open windows
- `workspace` - setting status text

## Data Access (`bpy.data`)

- `data` - how does it differ from `bpy.context.blend_data`?

## Operators (`bpy.ops`)

### UI

- `copy_python_command_button` - get python command name from button

## Utilities (`bpy.utils`)

- `blend_paths` - gets paths to referenced but unpacked files
- `execfile`

## Font Drawing (`blf`)

Could be used for the light box.

## To-Do

### Capture the subcontexts of the context access section

### Demo select API methods practically in auxiliary repos

### Go through all the types in the Types section and learn what they do

### Scrape the API docs automatically and cross-reference with my content

All API bits would have their own readme section automatically generated
and I would just fill in bits to the sections I played around with and
found something I wanted to capture.
