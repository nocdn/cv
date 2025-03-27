<script>
  const skillCategories = [
    {
      name: "Languages",
      skills: ["Python", "JavaScript", "Java", "Bash", "HTML", "SQL"],
    },
    {
      name: "Frameworks",
      skills: ["Svelte", "SvelteKit", "Tailwind CSS", "Flask", "Vite"],
    },
    {
      name: "Databases",
      skills: ["PostgreSQL", "SQLite", "Supabase"],
    },
    {
      name: "DevOps",
      skills: ["Nginx", "Linux administration", "Docker", "Virtualbox"],
    },
    {
      name: "Cloud",
      skills: [
        "AWS (Lambda, RDS, API Gateway, EC2)",
        "GCP",
        "Azure",
        "Oracle Cloud Infrastructure",
      ],
    },
    {
      name: "VCS & Workflow",
      skills: [
        "Git",
        "Agile methodologies",
        "GitHub Actions",
        "CI/CD understanding",
      ],
    },
    {
      name: "Soft Skills",
      skills: [
        "Teamwork",
        "Communication",
        "Creative thinking",
        "Adaptability",
        "Problem solving",
      ],
    },
  ];
</script>

<main class="flex flex-col gap-4">
  <p class="text-2xl font-bold">Skills</p>
  <div class="flex flex-col gap-2">
    {#each skillCategories as category}
      <div class="grid grid-cols-[20%_80%] gap-1.5">
        <p class="font-medium text-md font-geist-mono">{category.name}</p>
        <div class="flex gap-2 flex-wrap">
          {#each category.skills as skill}
            <span
              class="font-geist font-medium text-sm bg-gray-100 px-2 py-1 rounded-md group-hover:bg-gray-200 transition-all"
            >
              {skill}
            </span>
          {/each}
        </div>
      </div>
    {/each}
  </div>
</main>
