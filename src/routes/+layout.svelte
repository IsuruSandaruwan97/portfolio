<script lang="ts">
	import '../app.postcss';
	import ComingSoon from '../features/coming-soon/index.svelte';

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
</script>

<ComingSoon />

<slot />
