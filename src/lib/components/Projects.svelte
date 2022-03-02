<script lang="ts">
  interface Links {
    name: string
    demo?: string
    github: string
  }
  export let links: Links[] = []
</script>

<div class="w-fit sm:w-3/4 h-1/2 sm:h-auto flex flex-col sm:flex-row overflow-auto no-scrollbar">
  {#each links as { name, demo, github }}
    <div
      class="shrink-0 flex flex-col mx-0 sm:mx-4 my-2 sm:my-4 justify-center items-center gap-2 border-2 px-8 py-6 rounded-lg border-cyan-700 dark:border-cyan-200"
    >
      <h3 class="text-base sm:text-xl font-medium text-cyan-800 dark:text-cyan-200">{name}</h3>
      {#if demo}
        <a
          href={demo}
          target="_blank"
          rel="noreferrer"
          class="underline text-blue-800 dark:text-blue-200">[Live Demo]</a
        >
      {/if}
      <a
        href={github}
        target="_blank"
        rel="noreferrer"
        class="underline text-blue-800 dark:text-blue-200">[GitHub]</a
      >
    </div>
  {/each}
</div>
