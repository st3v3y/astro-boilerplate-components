<script lang="ts">
  import type { IFrontmatter } from '../types/IFrontMatter';

  export let content: IFrontmatter;
</script>

<div class="mx-auto mt-5 max-w-prose">
  <div class="aspect-w-3 aspect-h-2">
    <img
      class="h-full w-full rounded-lg object-cover object-center"
      src={content.imgSrc}
      alt={content.imgAlt}
      loading="lazy"
    />
  </div>

  <div class="prose prose-invert mt-8 prose-img:rounded-lg">
    <slot />
  </div>
</div>
