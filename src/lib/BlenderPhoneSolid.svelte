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
  export let ariaLabel = 'blender phone solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 20 18"
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
    d="M5.022 4.764c.489 0 .75-.37.8-.856l.188-1.877A.952.952 0 0 0 5.063.985H2.791a1.127 1.127 0 0 0-1.067.749A16.109 16.109 0 0 0 1 7a16.737 16.737 0 0 0 .743 5.242c.154.463 1.748.773 2.236.773H5a.95.95 0 0 0 .946-1.046l-.188-1.877a.95.95 0 0 0-.946-.856h-.761A14.627 14.627 0 0 1 3.937 7c-.02-.747.019-1.495.114-2.236h.971Zm13.365 7.592L18.6 11H14a1 1 0 0 1 0-2h4.918l.159-1H14a1 1 0 1 1 0-2h5.393l.158-1H14a1 1 0 1 1 0-2h5.868l.111-.7a2.04 2.04 0 0 0-.473-1.629A1.912 1.912 0 0 0 18.063 0H9a1 1 0 0 0-1 1v11.78A2.985 2.985 0 0 0 7 15v2a1 1 0 0 0 1 1h11a1 1 0 0 0 1-1v-2a2.99 2.99 0 0 0-1.613-2.644Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'blender phone solid';
-->
