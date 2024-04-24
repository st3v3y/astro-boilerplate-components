<script lang="ts">
  import type { Values } from '../types/TypeUnion';
  import { ColorTags, colorToClassMap } from '../types/ColorTags';

  export let color: Values<typeof ColorTags>;
</script>

<div class={`rounded-md px-2 py-1 text-xs font-semibold ${
      colorToClassMap[props.color]
    }`}
  >
  <slot />
</div>

