<script>
  let { title, description, demo = "", repo, upToDate = true } = $props();
  import { BadgeCheck } from "lucide-svelte";
  let showPopover = $state(false);
  let isLeaving = $state(false);

  function handleMouseLeave() {
    isLeaving = true;
    setTimeout(() => {
      showPopover = false;
      isLeaving = false;
    }, 200);
  }
</script>

<project
  class="flex flex-col gap-2 border border-gray-200 rounded-xl px-3.5 py-3"
>
  <div class="flex justify-between items-center">
    <p
      class="font-geist text-[17px] font-medium inline-flex items-center gap-2"
    >
      {title}
      <span
        role="tooltip"
        class="relative {upToDate ? 'block' : 'hidden'}"
        onfocus={() => {
          showPopover = true;
          isLeaving = false;
        }}
        onmouseover={() => {
          showPopover = true;
          isLeaving = false;
        }}
        onmouseleave={handleMouseLeave}
      >
        <BadgeCheck class="text-blue-700" size={16} strokeWidth={2.65} />
        {#if showPopover}
          <!-- svelte-ignore node_invalid_placement_ssr -->
          <div
            class="w-52 h-fit absolute bottom-6 left-1/2 -translate-x-1/2 bg-white rounded-xl border border-gray-200 shadow-xl z-10 p-3 font-geist-mono text-sm {isLeaving
              ? 'animate-preview-popover-down'
              : 'animate-preview-popover-up'}"
          >
            <p class="text-center">
              This project is currently actively <span
                class="text-blue-800 font-semibold">maintained.</span
              >
            </p>
          </div>
        {/if}
      </span>
    </p>
    <div class="flex gap-3 items-center">
      <a
        href={repo}
        target="_blank"
        rel="noopener noreferrer"
        class="text-sm font-geist-mono text-gray-500 hover:text-gray-700"
        >Repo</a
      ><a
        href={demo}
        target="_blank"
        rel="noopener noreferrer"
        class="text-sm font-geist-mono text-blue-700 hover:text-blue-600 {demo !==
        ''
          ? 'block'
          : 'hidden'}">Demo</a
      >
    </div>
  </div>
  <p class="font-geist-mono text-[15px]">{description}</p>
</project>
