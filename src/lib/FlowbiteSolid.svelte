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
  export let ariaLabel = 'flowbite solid';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  fill="currentColor"
  {...$$restProps}
  class={twMerge('shrink-0', sizes[size], $$props.class)}
  {role}
  aria-label={ariaLabel}
  viewBox="0 0 22 22"
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
    d="M15 11 9.186 8.093a.932.932 0 0 1-.166-.039L9 8.047v6.885c0 .018.009.036.011.054l2.49-3.125L15 11Z"
  />
  <path
    fill="currentColor"
    d="m10.366 2.655 5.818 3.491a4.2 4.2 0 0 1 1.962 3.969 3.237 3.237 0 0 1-2.393 2.732c-.024.007-.048.005-.073.011-.065.032-.132.06-.2.084l-2.837.7-2.077 2.606a1.99 1.99 0 0 1-.7.56c.05.036.09.081.144.113a2.126 2.126 0 0 0 2.08.037c.618-.348 2.242-1.262 4.836-3.038l.291-.2c1.386-.94 3.772-2.565 4.138-4.428A10.483 10.483 0 0 0 6.869 1.349c1.211.302 2.385.74 3.497 1.306Z"
  />
  <path
    fill="currentColor"
    d="M4.023 16.341V9.558A3.91 3.91 0 0 1 5.784 6.3a4.062 4.062 0 0 1 3.58-.257c.184.031.362.088.53.169l6 3c.086.052.168.11.246.174a2.246 2.246 0 0 0-.994-1.529L9.4 4.407c-1.815-.9-4.074-1.6-5.469-1.152a10.46 10.46 0 0 0 .534 15.953 18.148 18.148 0 0 1-.442-2.867Z"
  />
  <path
    fill="currentColor"
    d="m18.332 15.376-.283.192c-2.667 1.827-4.348 2.773-4.9 3.083a4.234 4.234 0 0 1-2.085.556 4.092 4.092 0 0 1-2.069-.561 3.964 3.964 0 0 1-1.951-3.373A1.917 1.917 0 0 1 7 15V8c0-.025.009-.049.01-.074A1.5 1.5 0 0 0 6.841 8a1.882 1.882 0 0 0-.82 1.592v6.7c.072 1.56.467 3.087 1.16 4.486A10.473 10.473 0 0 0 21.3 13.047a20.483 20.483 0 0 1-2.968 2.329Z"
  />
</svg>

<!--
@component
[Go to docs](https://flowbite-svelte-icons.vercel.app/)
## Props
@prop export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
@prop export let role: string = 'img';
@prop export let ariaLabel = 'flowbite solid';
-->
