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
  export let ariaLabel = 'dna solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 12 20"
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
    d="M11 0a1 1 0 0 0-1 1v1H2V1a1 1 0 0 0-2 0v3.169a5.966 5.966 0 0 0 2.269 4.7A1.001 1.001 0 1 0 3.513 7.3a3.756 3.756 0 0 1-.3-.3h5.608a4 4 0 0 1-.76.6l-5.148 3.087A6.027 6.027 0 0 0 0 15.831V19a1 1 0 1 0 2 0v-1h8v1a1 1 0 0 0 2 0v-3.169a5.979 5.979 0 0 0-.416-2.167 1.01 1.01 0 0 0-.044-.1 6.007 6.007 0 0 0-1.891-2.494 1 1 0 0 0-1.216 1.588c.125.107.244.222.354.344h-5.6a3.97 3.97 0 0 1 .76-.6l5.145-3.088a6.015 6.015 0 0 0 2.474-2.906c.009-.02.013-.041.021-.062A5.961 5.961 0 0 0 12 4.169V1a1 1 0 0 0-1-1ZM2 16v-.169c.003-.28.037-.558.1-.831h7.8c.062.273.096.551.1.831V16H2Zm8-12v.169c-.003.28-.037.558-.1.831H2.094A3.964 3.964 0 0 1 2 4.169V4h8Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'dna solid';
-->
