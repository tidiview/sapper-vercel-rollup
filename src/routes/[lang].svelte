<script context="module">
  export function preload (page) {
    return { lang: page.params.lang };
  }
</script>

<script>
  export let lang;
  const expressions = {
      "fr": "Je t'aime",
      "ja": "私は貴方を愛している",
      "en": "I love you"
    };
  const expression = expressions[lang];
</script>

<svelte:head>
  <title>{lang}</title>
</svelte:head>

<p>{expression}</p>