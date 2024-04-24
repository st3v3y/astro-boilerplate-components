<script lang="ts">
  export let title: string | undefined = undefined;
</script>

<div class="mx-auto max-w-screen-lg px-3 py-6">
  {#if title}
    <div class="mb-6 text-2xl font-bold">{title}</div>
  {/if}

  <slot />
</div>

