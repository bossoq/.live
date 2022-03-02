<script lang="ts">
  import IconButton from '$lib/components/IconButton.svelte'
  import GithubIcon from '$lib/components/Icons/GithubIcon.svelte'
  import BriefcaseIcon from '$lib/components/Icons/BriefcaseIcon.svelte'
  import ProjectIcon from '$lib/components/Icons/ProjectIcon.svelte'
</script>

<div class="flex flex-col sm:flex-row flex-wrap justify-center font-medium">
  <IconButton href="https://github.com/bossoq"
    ><span class="fill-balck dark:fill-white"><GithubIcon /></span>GitHub</IconButton
  >
  <IconButton href="https://resume.bossoq.live"
    ><span class="fill-balck dark:fill-white"><BriefcaseIcon /></span>Résumé</IconButton
  >
  <IconButton href="/projects"
    ><span class="fill-balck dark:fill-white"><ProjectIcon /></span>Projects</IconButton
  >
</div>
