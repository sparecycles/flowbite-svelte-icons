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
  export let ariaLabel = 'reply all solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 20 14"
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
  <g fill="currentColor">
    <path
      d="M13.606 3.748V2.531a1.542 1.542 0 0 0-.872-1.431 1.352 1.352 0 0 0-1.472.2L6.155 5.552a1.6 1.6 0 0 0 0 2.415l5.108 4.25a1.354 1.354 0 0 0 1.472.2 1.546 1.546 0 0 0 .872-1.428V9.9a4.72 4.72 0 0 1 3.7 2.867 1.187 1.187 0 0 0 1.08.731 1.225 1.225 0 0 0 1.213-1.287v-1.329a6.923 6.923 0 0 0-5.994-7.134Z"
    />
    <path
      d="m2.434 6.693 5.517-4.949A1 1 0 0 0 6.615.256L1.1 5.205a2.051 2.051 0 0 0-.01 3.035l5.61 5.088a1.001 1.001 0 0 0 1.344-1.482l-5.61-5.153Z"
    />
  </g>
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'reply all solid';
-->
