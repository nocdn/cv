<script>
  import Header from "./Header.svelte";
  import Summary from "./Summary.svelte";
  import Experience from "./Experience.svelte";
  import Education from "./Education.svelte";
  import Projects from "./Projects.svelte";
  import Skills from "./Skills.svelte";
  import Extras from "./Extras.svelte";
</script>

<main
  class="max-w-[21cm] mx-auto flex flex-col gap-8 not-print:pt-16 print:pt-5 pb-16"
>
  <Header />
  <Summary />
  <Experience />
  <Education />
  <Projects />
  <Skills />
  <Extras />
</main>
