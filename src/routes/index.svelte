<script>
  import { t, locale } from 'svelte-intl-precompile';
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<p>Translation1: {$t("menu")}</p>
<p>Translation2: {$t("foot", { values: { count: 2 } })}</p>

<button type="button" on:click={() => $locale = 'en'}>EN</button>
<button type="button" on:click={() => $locale = 'es'}>ES</button>