<script lang="ts">
  import { twMerge } from 'tailwind-merge';
  export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
  export let role: string = 'img';
  const sizes = {
    xs: 'w-3 h-3',
    sm: 'w-4 h-4',
    md: 'w-5 h-5',
    lg: 'w-6 h-6',
    xl: 'w-8 h-8'
  };
  export let ariaLabel = 'expand solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 18 18"
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
>
  <path
    fill="currentColor"
    d="M18 .989a1.016 1.016 0 0 0-.056-.277c-.011-.034-.009-.073-.023-.1a.786.786 0 0 0-.066-.1.979.979 0 0 0-.156-.224l-.007-.01a.873.873 0 0 0-.116-.073.985.985 0 0 0-.2-.128.959.959 0 0 0-.231-.047A.925.925 0 0 0 17 0h-4a1 1 0 1 0 0 2h1.664l-3.388 3.552a1 1 0 0 0 1.448 1.381L16 3.5V5a1 1 0 0 0 2 0V.989ZM17 12a1 1 0 0 0-1 1v1.586l-3.293-3.293a1 1 0 0 0-1.414 1.414L14.586 16H13a1 1 0 0 0 0 2h4a1 1 0 0 0 1-1v-4a1 1 0 0 0-1-1ZM3.414 2H5a1 1 0 0 0 0-2H1a1 1 0 0 0-1 1v4a1 1 0 0 0 2 0V3.414l3.536 3.535A1 1 0 0 0 6.95 5.535L3.414 2Zm2.139 9.276L2 14.665V13a1 1 0 1 0-2 0v4c.006.046.015.09.027.135.006.08.022.16.048.235a.954.954 0 0 0 .128.2.95.95 0 0 0 .073.117l.01.007A.983.983 0 0 0 1 18h4a1 1 0 0 0 0-2H3.5l3.436-3.276a1 1 0 0 0-1.38-1.448h-.003Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'expand solid';
-->
