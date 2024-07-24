<script lang="ts">
	import '../app.postcss';
	import Navbar from '../components/navbar/index.svelte';
	import Home from '../features/home/index.svelte';

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
</script>

<Navbar />
<Home />
<slot />
