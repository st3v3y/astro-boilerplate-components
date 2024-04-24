<script lang="ts">
  export let src: string;
  export let alt: string;
</script>

<img
  class="h-12 w-12 hover:translate-y-1"
  src={src}
  alt={alt}
  loading="lazy"
/>
