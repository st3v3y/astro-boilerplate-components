<script lang="ts">
  export let href: string;
  export let target: '_blank' | '_self' | '_parent' | '_top' | string;
</script>

<li class="hover:text-white">
  <a href={href} target={target || '_self'}>
    <slot />
  </a>
</li>
