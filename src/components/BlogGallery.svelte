<script lang="ts">
  import type { MarkdownInstance } from 'astro';
  import type { IFrontmatter } from '../types/IFrontMatter';
  import BlogCard from './BlogCard.svelte';

  let postList: MarkdownInstance<IFrontmatter>[];
</script>

<div class="grid grid-cols-1 gap-6 md:grid-cols-3">
  {#each postList as post}
    <BlogCard instance={post} />
  {/each}
</div>

