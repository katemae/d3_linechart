<script>
  import ChartContainer from "./components/ChartContainer.svelte";
  import { energy } from "./data/energy";
</script>

<main>
  <ChartContainer
    type={"lineChart"}
    chartProps={{
      data: energy,
      xVar: "year",
      yVars: [
        "biofuel",
        "coal",
        "fossil",
        "gas",
        "hydro",
        "nuclear",
        "oil",
        "solar"
      ],
    }}
  />
</main>