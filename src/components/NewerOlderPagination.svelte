<script lang="ts">
  import type { FrontmatterPage } from '../types/IFrontMatter';

  export let page: FrontmatterPage;
</script>

<div class="flex justify-center gap-8">
  {#if page.url.prev}
    <a href={page.url.prev}>← Newer Posts</a>
  {/if}
  {#if page.url.next}
    <a href={page.url.next}>Older Posts →</a>
  {/if}
</div>
