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
  export let ariaLabel = 'list ordored solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 21 18"
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
    d="M9.5 4h9.563a1 1 0 1 0 0-2H9.5a1 1 0 0 0 0 2Zm9.563 4H9.5a1 1 0 0 0 0 2h9.563a1 1 0 1 0 0-2Zm0 6H9.5a1 1 0 0 0 0 2h9.563a1 1 0 0 0 0-2ZM6.5 16H4.49l.871-.657a1.03 1.03 0 0 0 .121-.09A3 3 0 1 0 .5 13a1 1 0 1 0 2 0 1 1 0 1 1 1.7.713L.9 16.2a1 1 0 0 0 .6 1.8h5a1 1 0 0 0 0-2Zm-5-10a1 1 0 0 0 0 2h4a1 1 0 0 0 0-2h-1V1c0-.011-.006-.02-.006-.03a.961.961 0 0 0-.04-.2A1 1 0 0 0 4.4.582c0-.01 0-.02-.008-.03a1.064 1.064 0 0 0-.087-.111.985.985 0 0 0-.135-.172 1 1 0 0 0-.153-.1 1.016 1.016 0 0 0-.17-.1.943.943 0 0 0-.205-.041A.908.908 0 0 0 3.5 0c-.011 0-.02 0-.031.006a1.06 1.06 0 0 0-.191.038 1.047 1.047 0 0 0-.2.053c-.009 0-.02 0-.029.008l-2 1a1 1 0 1 0 .894 1.789l.557-.276V6h-1Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'list ordored solid';
-->
