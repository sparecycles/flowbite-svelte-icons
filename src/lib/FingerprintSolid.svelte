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
  export let ariaLabel = 'fingerprint solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 22 20"
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
      d="M20 9a1 1 0 0 0-1 1 27.238 27.238 0 0 1-1.042 8.693.999.999 0 1 0 1.903.614A28.898 28.898 0 0 0 21 10a1 1 0 0 0-1-1ZM6.762 3.217A7.969 7.969 0 0 1 11 2a8.052 8.052 0 0 1 7.21 4.536 1 1 0 0 0 1.8-.869A10.068 10.068 0 0 0 11 0a9.955 9.955 0 0 0-5.3 1.523 1 1 0 1 0 1.062 1.694ZM2.954 13.1c.007-.081.046-.6.046-3.1a7.929 7.929 0 0 1 1.542-4.716A1 1 0 0 0 2.928 4.1 9.916 9.916 0 0 0 1 10c0 2.375-.035 2.881-.038 2.913A1 1 0 0 0 1.861 14c.033 0 .066.005.1.005a1 1 0 0 0 .993-.905ZM17.5 7.41a1 1 0 0 0-1.857.742A4.96 4.96 0 0 1 16 10a29.23 29.23 0 0 1-.443 6.03 1 1 0 0 0 1.959.4c.386-2.12.548-4.276.484-6.43 0-.887-.17-1.767-.5-2.59Z"
    />
    <path
      d="M11 3a7.008 7.008 0 0 0-7 7 1 1 0 1 0 2 0 5 5 0 0 1 7.792-4.146A1 1 0 1 0 14.913 4.2 6.962 6.962 0 0 0 11 3Zm-6.011 9.766a1 1 0 0 0-1.176.785 4.16 4.16 0 0 1-.637 1.566A6.96 6.96 0 0 0 2 19a1 1 0 1 0 2 0 4.968 4.968 0 0 1 .841-2.771 6.154 6.154 0 0 0 .935-2.286 1 1 0 0 0-.787-1.177Zm8.711 2.496a1.002 1.002 0 0 0-1.212.729c-.211.859-.51 1.694-.894 2.491a1.001 1.001 0 0 0 1.434 1.28 1 1 0 0 0 .368-.413c.44-.92.786-1.883 1.03-2.874a1 1 0 0 0-.726-1.213Z"
    />
    <path
      d="M11 6a4 4 0 0 0-4 4c0 2.78 0 4.789-1.328 6.781a1 1 0 0 0 1.664 1.11C9 15.4 9 12.9 9 10a2 2 0 1 1 4 0c0 .736 0 1.495-.03 2.272a1 1 0 0 0 .96 1.039h.04a1 1 0 0 0 1-.961c.03-.804.03-1.588.03-2.35a4 4 0 0 0-4-4Z"
    />
    <path
      d="M11 9a1 1 0 0 0-1 1c0 2.93 0 5.7-1.832 8.445a1 1 0 0 0 1.664 1.11C12 16.3 12 13.1 12 10a1 1 0 0 0-1-1Z"
    />
  </g>
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'fingerprint solid';
-->
