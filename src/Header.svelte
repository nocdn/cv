<script>
  import picture from "/picture.jpg";
  import { MapPin, Github, Mail, Printer } from "lucide-svelte";
</script>

<header class="flex justify-between gap-16">
  <div class="flex flex-col gap-3">
    <p class="text-3xl font-bold">Bartosz Bak</p>
    <p class="font-geist-mono text-lg group">
      Student and an <span
        class="group-hover:text-blue-800 group-hover:font-medium transition-all"
        >aspiring</span
      >
      full-stack
      <span
        class="group-hover:text-blue-800 group-hover:font-medium transition-all"
        >software engineer</span
      > who likes to craft nice things.
    </p>
    <p class="flex gap-2 items-center font-geist-mono text-md text-gray-500">
      <MapPin size={16} /> York, United Kingdom, UTC
    </p>

    <div class="flex gap-5 items-center">
      <a
        href="https://github.com/nocdn"
        class="flex gap-2 items-center font-geist-mono text-md text-gray-700 transition-colors hover:text-blue-800"
      >
        <Github size={16} /> github.com/nocdn
      </a>
      <a
        href="mailto:contact@bartoszbak.org"
        class="flex gap-2 items-center font-geist-mono text-md text-gray-700 transition-colors hover:text-blue-800"
      >
        <Mail size={16} /> contact@bartoszbak.org
      </a>
      <!-- svelte-ignore a11y_invalid_attribute -->
      <a
        href="#"
        onclick={() => {
          window.print();
        }}
        class="flex gap-2 items-center font-geist-mono text-md text-gray-700 transition-colors hover:text-blue-800 print:hidden"
      >
        <Printer size={16} /> print
      </a>
    </div>
  </div>
  <div
    class="flex-shrink-0 w-36 h-36 mr-8 transition-all duration-300 overflow-hidden rounded-4xl border-2 border-gray-200"
  >
    <img
      src={picture}
      alt="Bartosz Bak"
      class="w-full h-full object-cover transition-transform duration-300 hover:scale-110"
      style="transition-timing-function: cubic-bezier(0.165, 0.84, 0.44, 1);"
    />
  </div>
</header>
