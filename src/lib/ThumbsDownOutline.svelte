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
  export let strokeLinecap: 'round' | 'inherit' | 'butt' | 'square' | null | undefined = 'round';
  export let strokeLinejoin: 'round' | 'inherit' | 'miter' | 'bevel' | null | undefined = 'round';
  export let strokeWidth = '2';
  export let ariaLabel = 'thumbs down outline';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="none"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 20 20"
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
    stroke="currentColor"
    stroke-linecap={strokeLinecap}
    stroke-linejoin={strokeLinejoin}
    stroke-width={strokeWidth}
    d="M15.992 11.287c-1 .097-1.96.45-2.792 1.029a25.118 25.118 0 0 0-4.454 5.721 1.803 1.803 0 0 1-.655.705 1.742 1.742 0 0 1-1.648.096 1.786 1.786 0 0 1-.604-.457 1.874 1.874 0 0 1-.432-1.439l1.562-4.626m9.023-1.03H19V2.03c0-.273-.106-.535-.294-.728A.99.99 0 0 0 17.997 1h-1.002a.99.99 0 0 0-.71.301 1.042 1.042 0 0 0-.293.728v9.258Zm-8.02 1.03H3.003c-.322 0-.64-.08-.925-.233a2.022 2.022 0 0 1-.716-.645 2.108 2.108 0 0 1-.242-1.883l2.36-7.2C3.769 1.54 3.96 1 5.365 1c2.59 0 5.39 1.06 7.504 1.66"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let strokeLinecap: 'round' | 'inherit' | 'butt' | 'square' | null | undefined = 'round';
@prop export let strokeLinejoin: 'round' | 'inherit' | 'miter' | 'bevel' | null | undefined = 'round';
@prop export let strokeWidth = '2';
@prop export let ariaLabel = 'thumbs down outline';
-->
