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
  export let ariaLabel = 'file shield solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 20 21"
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
      d="M6.167 9.833a3 3 0 0 1 1.946-2.809L13 5.191a3 3 0 0 1 2.107 0l.893.334V2a1.97 1.97 0 0 0-1.933-2H7v5a2 2 0 0 1-2 2H0v11a1.969 1.969 0 0 0 1.933 2h8.641A14.03 14.03 0 0 1 6.167 9.833Z"
    />
    <path
      d="M5 5V.13a2.96 2.96 0 0 0-1.293.749L.879 3.707A2.96 2.96 0 0 0 .13 5H5Zm14.3 3.9-4.893-1.837a1.009 1.009 0 0 0-.7 0L8.815 8.9a1 1 0 0 0-.648.936 12.263 12.263 0 0 0 5.359 10.015 1 1 0 0 0 1.06 0 12.265 12.265 0 0 0 5.358-10.015A1 1 0 0 0 19.3 8.9Zm-5.236 8.866V9.068l3.866 1.45a10.241 10.241 0 0 1-3.871 7.245l.005.003Z"
    />
  </g>
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'file shield solid';
-->
