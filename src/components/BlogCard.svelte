<script lang="ts">
  import type { MarkdownInstance } from 'astro';
  import { format } from 'date-fns';

  import type { IFrontmatter } from '../types/IFrontMatter';

  export let instance: MarkdownInstance<IFrontmatter>;
</script>

<a class="hover:translate-y-1" href={instance.url}>
  <div class="overflow-hidden rounded-md bg-slate-800">
    <div class="aspect-w-3 aspect-h-2">
      <img
        class="h-full w-full object-cover object-center"
        src={instance.frontmatter.imgSrc}
        alt={instance.frontmatter.imgAlt}
        loading="lazy"
      />
    </div>

    <div class="px-3 pt-4 pb-6 text-center">
      <h2 class="text-xl font-semibold">
        {instance.frontmatter.title}
      </h2>

      <div class="mt-1 text-xs text-gray-400">
        {format(new Date(instance.frontmatter.pubDate), 'LLL d, yyyy')}
      </div>

      <div class="mt-2 text-sm">
        {instance.frontmatter.description}
      </div>
    </div>
  </div>
</a>
