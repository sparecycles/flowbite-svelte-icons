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
  export let ariaLabel = 'face grin outline';
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
    fill="currentColor"
    d="m4.985 10.995.72-.694a1 1 0 0 0-1.72.694h1Zm10.034 0h1a1 1 0 0 0-1.694-.72l.694.72ZM6.5 6.5a1 1 0 0 0 0 2v-2Zm.01 2a1 1 0 0 0 0-2v2Zm6.99-2a1 1 0 1 0 0 2v-2Zm.01 2a1 1 0 1 0 0-2v2ZM18 10a8 8 0 0 1-8 8v2c5.523 0 10-4.477 10-10h-2Zm-8 8a8 8 0 0 1-8-8H0c0 5.523 4.477 10 10 10v-2Zm-8-8a8 8 0 0 1 8-8V0C4.477 0 0 4.477 0 10h2Zm8-8a8 8 0 0 1 8 8h2c0-5.523-4.477-10-10-10v2Zm-5.735 9.69c.601.622 1.578.962 2.504 1.16.978.21 2.114.304 3.23.298 1.116-.006 2.25-.112 3.225-.323.925-.2 1.89-.531 2.49-1.11l-1.39-1.44c-.173.168-.66.408-1.523.595-.813.176-1.804.273-2.813.278-1.008.005-1.996-.082-2.8-.254-.857-.183-1.322-.425-1.484-.593L4.265 11.69Zm9.754-.695c0 .368-.283 1.325-1.012 2.207-.692.838-1.692 1.492-3.038 1.492v2c2.08 0 3.604-1.037 4.58-2.218.94-1.14 1.47-2.532 1.47-3.48h-2Zm-4.05 3.699c-1.353 0-2.334-.638-3.003-1.456-.702-.858-.981-1.815-.981-2.243h-2c0 .978.5 2.37 1.433 3.51.967 1.18 2.479 2.189 4.55 2.189v-2ZM6.5 8.5h.01v-2H6.5v2Zm7 0h.01v-2h-.01v2Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'face grin outline';
-->
