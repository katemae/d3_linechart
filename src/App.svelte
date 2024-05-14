<script>
  import ChartContainer from "./components/ChartContainer.svelte";
  import { energy } from "./data/energy";
</script>

<main>
  <h1>Energy Generation</h1>

	<p>...</p>

  <div class="chart">
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
	</div>
</main>

<style>
	h1 {
		text-align: center;
	}

	p {
		text-align: center;
	}

	.chart {
		text-align: center;
	}
</style>