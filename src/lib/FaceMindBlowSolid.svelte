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
  export let ariaLabel = 'face mind blow solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
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
    fill="currentColor"
    d="M19.472 9.541a.5.5 0 0 0-.982-.1 1.308 1.308 0 0 1-1.258.96 1.394 1.394 0 0 1-1.329-.959.5.5 0 0 0-.965 0 1.394 1.394 0 0 1-2.6.136l-.046-.194.02-.139V7.5H14.5A2.5 2.5 0 0 0 17 5a2.544 2.544 0 0 0-2.521-2.5l-.5.021-.124-.351A2.5 2.5 0 0 0 11.5.5c-.439 0-.87.118-1.248.34L10 .987 9.748.84A2.472 2.472 0 0 0 8.5.5a2.5 2.5 0 0 0-2.358 1.671l-.124.351-.492-.022A2.547 2.547 0 0 0 3 5a2.5 2.5 0 0 0 2.5 2.5h2.229v1.793l-.007.085-.026.077a1.26 1.26 0 0 1-1.236.945 1.55 1.55 0 0 1-1.427-.972.5.5 0 0 0-.959.012 1.4 1.4 0 0 1-1.334.96 1.312 1.312 0 0 1-1.259-.96.52.52 0 0 0-.54-.363H.933a.5.5 0 0 0-.433.5V10a9.511 9.511 0 0 0 9.5 9.5 9.41 9.41 0 0 0 6.713-2.793 9.516 9.516 0 0 0 2.786-6.74l-.027-.426ZM6.5 13.5a1 1 0 1 1 2 0 1 1 0 0 1-2 0ZM8 17a2 2 0 0 1 4 0H8Zm4.5-2.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'face mind blow solid';
-->
