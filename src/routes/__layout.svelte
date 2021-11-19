<script context="module">
  import { addMessages, init, getLocaleFromNavigator, register } from 'svelte-intl-precompile';
  import en from '$locales/en.js';
  import es from '$locales/es.js';

  addMessages('en', en);
  addMessages('es', es);

  init({
    fallbackLocale: 'en',
    initialLocale: getLocaleFromNavigator()
  });
</script>

<slot />
