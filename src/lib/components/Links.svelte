<script lang="ts">
  import IconButton from './IconButton.svelte'
  import GithubIcon from './GithubIcon.svelte'
  import BriefcaseIcon from './BriefcaseIcon.svelte'
  import ProjectIcon from './ProjectIcon.svelte'
</script>

<div class="flex flex-col sm:flex-row flex-wrap justify-center font-medium">
  <IconButton href="https://github.com/bossoq"
    ><span class="fill-balck dark:fill-white"><GithubIcon /></span>GitHub</IconButton
  >
  <IconButton href="https://resume.bossoq.live"
    ><span class="fill-balck dark:fill-white"><BriefcaseIcon /></span>Résumé</IconButton
  >
  <IconButton href="#"
    ><span class="fill-balck dark:fill-white"><ProjectIcon /></span>Projects</IconButton
  >
</div>
