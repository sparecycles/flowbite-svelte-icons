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
  export let ariaLabel = 'dollar solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 11 20"
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
    d="M7.146 4.688c.808.18 1.54.608 2.093 1.224a1 1 0 0 0 1.522-1.3A5.991 5.991 0 0 0 7.62 2.744c-.208-.05-.413-.068-.62-.1V1.417a1 1 0 1 0-2 0v1.257a4.5 4.5 0 0 0-3.735 3.02A3.6 3.6 0 0 0 1.7 8.526 6.322 6.322 0 0 0 5.648 11.3c1.105.24 2.073.9 2.7 1.841a1.687 1.687 0 0 1 .235 1.284c-.352 1.273-2.16 1.978-3.954 1.542a3.962 3.962 0 0 1-2.108-1.243 1 1 0 1 0-1.535 1.283 5.964 5.964 0 0 0 3.169 1.9c.28.067.563.116.849.145v.864a1 1 0 1 0 2 0v-.976a4.456 4.456 0 0 0 3.507-2.984 3.607 3.607 0 0 0-.438-2.83 6.334 6.334 0 0 0-3.946-2.773 4.357 4.357 0 0 1-2.7-1.84 1.692 1.692 0 0 1-.235-1.285c.353-1.271 2.164-1.976 3.954-1.54Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'dollar solid';
-->
