<script lang="ts">
  import Projects from '$lib/components/Projects.svelte'
  import BackToHome from '$lib/components/BackToHome.svelte'

  const projectsList = [
    {
      name: 'ODD แ OUT',
      demo: 'https://odd-aer-out.bossoq.live',
      github: 'https://github.com/bossoq/odd-aer-out'
    },
    {
      name: 'สร้าง คำ เสี่ยว',
      demo: 'https://siewword.bossoq.live',
      github: 'https://github.com/bossoq/siew-generator'
    },
    {
      name: 'SET Market Return Calculator',
      demo: 'https://mktreturn.bossoq.live',
      github: 'https://github.com/bossoq/MarketStatisticsReact'
    },
    {
      name: 'Supapanya Tutoring School',
      demo: 'https://supapanya.com',
      github: 'https://github.com/bossoq/supapanya'
    },
    {
      name: 'Sniffslive Twitch Bot',
      github: 'https://github.com/Ponny035/SniffsLiveTwitchBot'
    },
    {
      name: 'Sniffslive Discord Bot',
      github: 'https://github.com/bossoq/SniffsbotDiscord'
    },
    {
      name: 'Sniffslive Webfeed',
      github: 'https://github.com/bossoq/SniffsbotWebfeed'
    }
  ]
</script>

<div class="w-full h-screen flex flex-col justify-center items-center bg-white dark:bg-black">
  <h1 class="text-3xl sm:text-6xl flex flex-row text-teal-800 dark:text-teal-200">Projects</h1>
  <span class="my-4" />
  <Projects links={projectsList} />
  <span class="my-4" />
  <BackToHome />
</div>
