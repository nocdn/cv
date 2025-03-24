<script>
  import { ArrowUpRight } from "lucide-svelte";
</script>

<main class="flex flex-col gap-4">
  <p class="text-2xl font-bold">Education</p>
  <div class="flex flex-col gap-1.5">
    <a
      href="https://www.york.ac.uk/study/undergraduate/courses/bsc-computer-science-industry/"
      target="_blank"
      class="font-semibold text-xl inline-flex items-center"
    >
      BSc Computer Science <ArrowUpRight
        size={20}
        class=" mt-0.75 ml-2 opacity-50"
      />
      <span class="ml-auto font-geist-mono text-sm font-normal opacity-75"
        >September 2024 - Present</span
      >
    </a>
    <p class="font-medium text-md font-geist-mono">
      University of York <span class="opacity-50">York, UK</span>
    </p>
    <p class="font-semibold">Relevant Modules:</p>
    <ul class="list-disc ml-6 text-sm space-y-1 font-geist-mono group">
      <li>
        <span class="group-hover:text-blue-800 transition-all font-semibold"
          >Object-Oriented Data Structures & Algorithms (Java):</span
        >
        Implementation of key data structures (stacks, queues, trees, graphs); Complexity
        analysis; Algorithm design paradigms (greedy, dynamic programming).
      </li>
      <li>
        <span class="group-hover:text-blue-800 transition-all font-semibold"
          >Foundations of Programming (Python):</span
        >
        procedural programming, data structures, file handling (JSON, CSV), debugging,
        unit-testing and version control.
      </li>
      <li>
        <span class="group-hover:text-blue-800 transition-all font-semibold"
          >Human-Computer Interaction:</span
        >
        user-centred design processes, iterative prototyping, usability assessment
        and inclusive design principles.
      </li>
      <li>
        <span class="group-hover:text-blue-800 transition-all font-semibold"
          >Mathematical Foundations:</span
        >
        discrete mathematics including combinatorics, probability, logic, set theory,
        graph theory.
      </li>
      <li>
        <span class="group-hover:text-blue-800 transition-all font-semibold"
          >Computer Systems and Architecture:</span
        >
        CPU/memory architecture, binary arithmetic, logical circuits, Von Neumann
        architecture, low-level programming (assembly and C), security implications
        in hardware.
      </li>
    </ul>
  </div>
</main>
