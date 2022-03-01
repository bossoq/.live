<script lang="ts">
  import Greeting from '$lib/components/Greeting.svelte'
  import Tagline from '$lib/components/Tagline.svelte'
  import Links from '$lib/components/Links.svelte'
</script>

<div class="w-full h-screen flex flex-col justify-center items-center bg-white dark:bg-black">
  <Greeting />
  <span class="my-4" />
  <Tagline />
  <span class="my-4" />
  <Links />
</div>
