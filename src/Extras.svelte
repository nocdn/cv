<script>
  import { ArrowUpRight, TicketsPlane } from "lucide-svelte";
  import Extra from "./lib/Extra.svelte";
</script>

<extra class="flex flex-col gap-4 group">
  <p class="text-2xl font-bold">Extra information</p>

  <Extra
    title="Morgan Stanley programming challenge"
    description="Collaborated in a team to develop an automated trading algorithm for a simulated currency market. Implemented real-time market analysis and decision-making logic in Python placing in the top ~25% of teams."
    link="https://morganstanley.tal.net/vx/lang-en-GB/candidate/postings/12379"
  />

  <Extra
    title="Microsoft Azure AI Hackathon"
    description="Enhanced the ad segment trimmer project with Azure AI Foundry, AI Speech and Elastic Compute. Implementing extra features like segment summaries, format conversions and an intuitive drag-and-drop frontend interface."
    link="https://azureaidev.devpost.com/"
  />

  <Extra
    title="Peer mentoring"
    description="Provided one-on-one mentoring to a sixth form student in A-level computer science and mathematics, creating personalised learning materials and exercises. Helped improve their understanding of algorithmic thinking, problem solving and programming."
    link="#"
  />
</extra>
