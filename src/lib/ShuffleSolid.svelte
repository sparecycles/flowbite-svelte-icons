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
  export let ariaLabel = 'shuffle solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 20 19"
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
      d="M19.923 13.618a1 1 0 0 0-.217-.326l-3-3a1 1 0 0 0-1.414 1.414L16.586 13h-3.065l-6.7-9.573A1 1 0 0 0 6 3H1a1 1 0 0 0 0 2h4.479l6.7 9.573A1 1 0 0 0 13 15h3.586l-1.293 1.293a1 1 0 1 0 1.414 1.414l3-3a1 1 0 0 0 .217-1.09l-.001.001Z"
    />
    <path
      d="M5.479 13H1a1 1 0 0 0 0 2h5a1 1 0 0 0 .819-.427l1.766-2.522-1.221-1.743L5.479 13Zm8.042-8H17l-1.8 2.4a1 1 0 0 0 1.6 1.2l3-4a.965.965 0 0 0 .058-.116 1.05 1.05 0 0 0 .075-.15.96.96 0 0 0 .046-.23A.92.92 0 0 0 20 4c0-.012-.006-.021-.007-.033a1.012 1.012 0 0 0-.054-.27c-.01-.031-.011-.066-.024-.1a1.024 1.024 0 0 0-.2-.29c-.005 0-.007-.012-.013-.018l-3-3a1 1 0 0 0-1.414 1.414L16.586 3H13a1 1 0 0 0-.819.427l-1.766 2.522 1.221 1.743L13.521 5Z"
    />
  </g>
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'shuffle solid';
-->
