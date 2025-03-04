<script lang="ts">
	import '../app.css';
	let { children } = $props();
	import '@fontsource-variable/roboto';
	import '@fontsource/konkhmer-sleokchher';
	import '@fontsource/krona-one';
	import Header from '../components/staticDirs/Header.svelte';
	import SubFooter from '../components/Footer/SubFooter.svelte';
	import Footer from '../components/Footer/Footer.svelte';
</script>
<div class="@container text-black font-main overflow-hidden flex flex-col min-h-screen gap-10 xl:gap-30">
	<Header />
	<main class="flex-1">{@render children()}</main>
	<div class="bg-darkBlue p-2 py-10">
		<SubFooter />
		<Footer />
	</div>
</div>
