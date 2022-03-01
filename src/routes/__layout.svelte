<script lang="ts">
  import '../app.css'
  import Head from '$lib/components/Head.svelte'
  import Menu from '$lib/components/Menu.svelte'
  import ThemeSelector from '$lib/components/ThemeSelector.svelte'
  import Modal from '$lib/components/Modal.svelte'
  import { darkTheme, modalViewed } from '$lib/store'

  const url = 'https://bossoq.live'
  const title = 'bossoq.live'
  const description = "Hello there, I'm bossoq."

  const menuItems = [{ name: 'Made by bossoq', url: 'https://github.com/bossoq/.live' }]
  const imageUrl = `${url}/screenshot.jpg`
  const gtagId = 'G-N0EVPLJVD3'
  const themeIcons = ['🌞 Toggle Light mode', '🌙 Toggle Dark mode']
</script>

<Head {title} {description} {url} {imageUrl} {gtagId} />
<main class={$darkTheme && 'dark'}>
  <ThemeSelector {themeIcons} />
  <Menu items={menuItems} />
  {#if $modalViewed}
    <Modal />
  {/if}
  <slot />
</main>
