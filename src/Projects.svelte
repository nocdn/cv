<script>
  import Project from "./lib/Project.svelte";
</script>

<main class="flex flex-col gap-4">
  <p class="text-2xl font-bold">Projects</p>
  <projects class="flex gap-3 flex-wrap">
    <row class="grid grid-cols-2 gap-3">
      <Project
        title="Transcriptions"
        description="Full-stack, self-hostable and containerised app for transcribing audio and video files with whisper, gemini, etc"
        demo="https://whisper.bartoszbak.org"
        repo="https://github.com/nocdn/transcriptions"
      />
      <Project
        title="Ad segment remover"
        description="Self-hostable and containerised RESTful API to intelligently remove advertisement segments from audio and video files."
        demo="https://segments.bartoszbak.org"
        repo="https://github.com/nocdn/ad-segment-trimmer"
      />
    </row>
    <row class="grid grid-cols-2 gap-3">
      <Project
        title="Voting"
        upToDate={false}
        description="Routed, sveltekit-based app for voting in a university society election. Also with Supabase and PostgreSQL."
        repo="https://github.com/nocdn/voting"
      />
      <Project
        title="Name sniper"
        description="Simple python script to check availability of usernames in a video game."
        repo="https://github.com/nocdn/namesniper"
      />
    </row>
  </projects>
</main>
