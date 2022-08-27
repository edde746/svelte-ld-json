<script>
  import LDtag from '$lib';
</script>

<main>
  <h1>Svelte LD+JSON</h1>
  <p>Easily add ld+json to your Svelte project</p>
  <span>Example:</span>
  <pre>
{`${'<'}script>
  import LDtag from 'svelte-ld-json';
</script>

<LDtag
  schema={{
    '@context': 'https://schema.org',
    '@type': 'Person',
    name: 'John Doe',
    url: 'https://example.com/',
    sameAs: ['https://twitter.com/johndoe', 'https://facebook.com/johndoe']
  }}
/>`}
</pre>
</main>

<!-- Example for page -->
<LDtag
  schema={{
    '@context': 'https://schema.org',
    '@type': 'Person',
    name: 'John Doe',
    url: 'https://example.com/',
    sameAs: ['https://twitter.com/johndoe', 'https://facebook.com/johndoe'],
  }}
/>

<style>
  main {
    font-family: sans-serif;
    max-width: 50rem;
    margin: 0 auto;
  }

  pre {
    background-color: #f5f5f5;
    border: 1px solid #ccc;
    padding: 1rem;
  }

  span {
    font-size: 0.75rem;
    color: rgb(80, 80, 80);
  }
</style>
