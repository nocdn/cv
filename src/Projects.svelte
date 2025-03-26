<script>
  import Project from "./lib/Project.svelte";
</script>

<main class="flex flex-col gap-4">
  <p class="text-2xl font-bold">Projects</p>
  <projects>
    <Project
      title="Transcriptions"
      description="Full-stack, self-hostable and containerised app for transcribing audio and video files with whisper, gemini, etc"
      demo="https://whisper.bartoszbak.org"
      repo="https://github.com/nocdn/transcriptions"
    />
  </projects>
</main>
