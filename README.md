# Svelte Accessible Range Input

[REPL Example](https://svelte.dev/repl/7f0042a186ee4d8e949c46ca663dbe6c?version=3.33.0)

A basic reference for an accessible range control that can be dropped in to your Svelte project.

No current intentions to turn this into a module, just grab copy the code and away you go. Check the REPL for an implementation example.

**Features**

- onChange Event / Value binding
- Custom Property theming
- Tooltip
- A11y Keyboard control / Labels

## Access value

You can retrieve the value from the control through either the onChange event
or binding the value to a parent variable.

onChange event listener: `<Range on:change={(e) => value = e.detail.value} />`

Bind value: `<Range bind:value/>`

## Theme Custom Properties

**Track**

`--track-focus`: Outline of track when tab-focused

`--track-bgcolor`: Non-active background color of track

`--track-highlight-bg-color`: Background color of active part of track

`--track-highlight-bg`: Background of active part of track, can use linear-gradient()

**Thumb**

`--thumb-bgcolor`: Background color of thumb

`--thumb-holding-outline`: rgba(x, x, x, 0.3) value for the circular outline on the thumb when held

**Tooltip**

`--tooltip-bgcolor`: Background color of tooltip

`--tooltip-bg`: Background of tooltip, can use linear-gradient()

`--tooltip-text`: Text color for tooltip
