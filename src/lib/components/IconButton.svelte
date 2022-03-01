<script lang="ts">
  export let href = '#'
  export let icon = ''
</script>

<a
  {href}
  class="flex mx-8 xs:mx-0 justify-center items-center gap-2 transition ease-in-out border-2 px-4 py-2 rounded border-slate-700 dark:border-slate-200 text-slate-800 hover:bg-slate-200 dark:text-slate-400 dark:hover:bg-slate-800"
>
  {#if icon}<span>{icon}</span>{/if}
  <slot />
</a>
