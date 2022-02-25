<script context="module">
	import pathsByName from "./icon-paths"
	export const iconOptions = Object.keys(pathsByName)
	export const directions = ["n", "ne", "e", "se", "s", "sw", "w", "nw"]
</script>
<script>
	export let name = "arrow"
	export let direction = "n"
	export let type = "outline"
	
	$: paths = pathsByName[type][name] || []
	$: rotation = directions.indexOf(direction) * 45
</script>
	
	<svg
		class={$$props.class ? $$props.class : 'h-6 w-6 overflow-visible'}
		fill={type == 'solid' ? "currentColor" : "none"}
		stroke={type == 'outline' ? "currentColor" : "none"}
		stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
		viewBox={type == 'solid' ? "0 0 20 20" : "0 0 24 24"}
		fill-rule="evenodd"
		clip-rule="evenodd"
		style="{`transform: rotate(${rotation}deg)`}">
		{#each paths as path}
			<path d="{path}"></path>
		{/each}
	</svg>
	  