<script>
  import { ArrowUpRight } from "lucide-svelte";
  let { title, description, link } = $props();
</script>

<div class="flex flex-col gap-1 border border-gray-200 rounded-xl px-3.5 py-3">
  <a class="font-semibold inline-flex items-center text-md" href={link}>
    {title}: <ArrowUpRight
      class="ml-auto -translate-y-0.5 opacity-50"
      size={18}
    />
  </a>
  <p class="font-geist text-sm">
    {description}
  </p>
</div>
