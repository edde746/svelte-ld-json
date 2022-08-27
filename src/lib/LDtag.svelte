<script lang="ts">
  import type { Thing, WithContext, Person } from 'schema-dts';
  const serializeSchema = (data: any) =>
    `<script type="application/ld+json">${JSON.stringify(data, null, 2)}${'<'}/script>`;
  export let schema: Thing | WithContext<Thing>;
</script>

<svelte:head>
  {@html serializeSchema(schema)}
</svelte:head>
