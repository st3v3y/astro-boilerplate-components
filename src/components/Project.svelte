<script lang="ts">
  export let img: { src: string; alt: string; };
  export let name: string;
  export let description: string;
  export let link: string;
  export let category: ReactNode;
</script>

<div class="flex flex-col items-center gap-x-8 rounded-md bg-slate-800 p-3 md:flex-row">
  <div class="shrink-0">
    <a href={link}>
      <img
        class="h-36 w-36 hover:translate-y-1"
        src={img.src}
        alt={img.alt}
        loading="lazy"
      />
    </a>
  </div>

  <div>
    <div class="flex flex-col items-center gap-y-2 md:flex-row">
      <a class="hover:text-cyan-400" href={link}>
        <div class="text-xl font-semibold">{name}</div>
      </a>

      <div class="ml-3 flex flex-wrap gap-2">
        <slot name="category"></slot>
      </div>
    </div>

    <p class="mt-3 text-gray-400">{description}</p>
  </div>
</div>
