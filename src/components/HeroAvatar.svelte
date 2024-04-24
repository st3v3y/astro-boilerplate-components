<script lang="ts">
  export let title: string;
  export let description: string;
</script>

<div class="flex flex-col items-center md:flex-row md:justify-between md:gap-x-24">
  <div>
    <h1 class="text-3xl font-bold">{title}</h1>

    <p class="mt-6 text-xl leading-9">{description}</p>

    <slot name="socialButtons" class="mt-3 flex gap-1" /> 
  </div>

  <slot name="avatar" class="shrink-0" /> 
</div>
