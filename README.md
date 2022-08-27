# svelte-ld-json

Easily add ld+json to your Svelte project

## Example

```html
<script>
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
/>
```

