<script lang="ts">
  import { format } from 'date-fns';
  import type { IFrontmatter } from '../types/IFrontMatter';

  export let content: IFrontmatter;
  export let author: string;
</script>

<h1 class="text-center text-3xl font-bold">{content.title}</h1>

<div class="mt-2 text-center text-sm text-gray-400">
  By {author} on{' '}
  {format(new Date(content.pubDate), 'LLL d, yyyy')}
</div>
