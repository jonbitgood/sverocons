# Sverocons

A simple svelte wrapper for the <a href="https://heroicons.com/" class="text-purple-800 bold">Heroicons Library</a> taking inspiration from the 
<a href="https://svelte.recipes/components/icon/">component approach</a> to svg icons by <a href="https://github.com/Wattenberger">Amelia Wattenberger</a>.

## Using an Icon

All icons can receive three different inputs:

- name
- type
- direction

Only Name is required with type defaulting to `outline` and and direction to `n`.
All directional icons have been removed IE arrow-right where they were identical.
The styles default to `h-6 w-6`, but this can be overridden by adding in a class.

```jsx
<Icon name="arrow" type="solid" direction="w" class="h-8 w-8" />
```