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
  export let ariaLabel = 'table row outline';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="none"
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
  <path
    fill="currentColor"
    d="M1 8a1 1 0 0 0 0 2V8Zm18 2a1 1 0 1 0 0-2v2ZM2 2h16V0H2v2Zm16 0h2a2 2 0 0 0-2-2v2Zm0 0v10h2V2h-2Zm0 10v2a2 2 0 0 0 2-2h-2Zm0 0H2v2h16v-2ZM2 12H0a2 2 0 0 0 2 2v-2Zm0 0V2H0v10h2ZM2 2V0a2 2 0 0 0-2 2h2Zm0 4h17V4H2v2Zm9 7V6H9v7h2ZM1 10h18V8H1v2Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'table row outline';
-->
