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
  export let ariaLabel = 'keyboard outline';
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
    d="M6.5 9.5v-1a1 1 0 0 0-1 1h1Zm7 0h1a1 1 0 0 0-1-1v1Zm0 1v1a1 1 0 0 0 1-1h-1Zm-7 0h-1a1 1 0 0 0 1 1v-1ZM4 4V3H3v1h1Zm0 .01H3v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V3h-1v1ZM4 7V6H3v1h1Zm0 .01H3v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V6h-1v1ZM4 10V9H3v1h1Zm0 .01H3v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V9h-1v1ZM7 4V3H6v1h1Zm0 .01H6v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V3h-1v1ZM7 7V6H6v1h1Zm0 .01H6v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V6h-1v1ZM10 4V3H9v1h1Zm0 .01H9v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V3h-1v1ZM10 7V6H9v1h1Zm0 .01H9v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V6h-1v1ZM13 4V3h-1v1h1Zm0 .01h-1v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V3h-1v1ZM13 7V6h-1v1h1Zm0 .01h-1v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V6h-1v1ZM16 7V6h-1v1h1Zm0 .01h-1v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V6h-1v1ZM16 10V9h-1v1h1Zm0 .01h-1v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V9h-1v1ZM16 4V3h-1v1h1Zm0 .01h-1v1h1v-1Zm.01 0v1h1v-1h-1Zm0-.01h1V3h-1v1ZM2 2h16V0H2v2Zm16 0h2a2 2 0 0 0-2-2v2Zm0 0v10h2V2h-2Zm0 10v2a2 2 0 0 0 2-2h-2Zm0 0H2v2h16v-2ZM2 12H0a2 2 0 0 0 2 2v-2Zm0 0V2H0v10h2ZM2 2V0a2 2 0 0 0-2 2h2Zm4.5 8.5h7v-2h-7v2Zm6-1v1h2v-1h-2Zm1 0h-7v2h7v-2Zm-6 1v-1h-2v1h2ZM3 4v.01h2V4H3Zm1 1.01h.01v-2H4v2Zm1.01-1V4h-2v.01h2ZM4.01 3H4v2h.01V3ZM3 7v.01h2V7H3Zm1 1.01h.01v-2H4v2Zm1.01-1V7h-2v.01h2ZM4.01 6H4v2h.01V6ZM3 10v.01h2V10H3Zm1 1.01h.01v-2H4v2Zm1.01-1V10h-2v.01h2ZM4.01 9H4v2h.01V9ZM6 4v.01h2V4H6Zm1 1.01h.01v-2H7v2Zm1.01-1V4h-2v.01h2ZM7.01 3H7v2h.01V3ZM6 7v.01h2V7H6Zm1 1.01h.01v-2H7v2Zm1.01-1V7h-2v.01h2ZM7.01 6H7v2h.01V6ZM9 4v.01h2V4H9Zm1 1.01h.01v-2H10v2Zm1.01-1V4h-2v.01h2Zm-1-1.01H10v2h.01V3ZM9 7v.01h2V7H9Zm1 1.01h.01v-2H10v2Zm1.01-1V7h-2v.01h2Zm-1-1.01H10v2h.01V6ZM12 4v.01h2V4h-2Zm1 1.01h.01v-2H13v2Zm1.01-1V4h-2v.01h2Zm-1-1.01H13v2h.01V3ZM12 7v.01h2V7h-2Zm1 1.01h.01v-2H13v2Zm1.01-1V7h-2v.01h2Zm-1-1.01H13v2h.01V6ZM15 7v.01h2V7h-2Zm1 1.01h.01v-2H16v2Zm1.01-1V7h-2v.01h2Zm-1-1.01H16v2h.01V6ZM15 10v.01h2V10h-2Zm1 1.01h.01v-2H16v2Zm1.01-1V10h-2v.01h2Zm-1-1.01H16v2h.01V9ZM15 4v.01h2V4h-2Zm1 1.01h.01v-2H16v2Zm1.01-1V4h-2v.01h2Zm-1-1.01H16v2h.01V3Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'keyboard outline';
-->
