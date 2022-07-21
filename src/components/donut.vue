<template>
  <div class="border border-gray-300 rounded p-5 m-5">
    <div class="flex justify-between">
      <div class="font-medium">Gender</div>
      <div class="flex items-center">
        <div class="text-sm">2022</div>
        <span class="px-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-3 w-3"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
              clip-rule="evenodd"
            /></svg
        ></span>
      </div>
    </div>
    <div class="hello" id="chartdiv"></div>
  </div>
</template>

<script>
import * as am4core from "@amcharts/amcharts4/core";
import * as am4charts from "@amcharts/amcharts4/charts";
import am4themes_animated from "@amcharts/amcharts4/themes/animated";

am4core.useTheme(am4themes_animated);
export default {
  mounted() {
    // Create chart instance
    var chart = am4core.create("chartdiv", am4charts.PieChart);

    // Add data
    chart.data = [
      {
        country: "Woman",
        value: 300,
        percent: "",
      },
      {
        country: "Man",
        value: 944,
        percent: "",
      },
    ];

    // Add and configure Series
    var pieSeries = chart.series.push(new am4charts.PieSeries());
    pieSeries.dataFields.value = "value";
    pieSeries.dataFields.category = "country";
    pieSeries.labels.template.disabled = true;
    pieSeries.ticks.template.disabled = true;

    pieSeries.colors.list = [
      am4core.color("#51b69e"),
      am4core.color("#4164cf"),
    ];

    chart.legend = new am4charts.Legend();
    chart.legend.position = "bottom";

    chart.innerRadius = am4core.percent(70);

    var label = pieSeries.createChild(am4core.Label);
    label.text = "{values.value.sum}";
    label.horizontalCenter = "middle";
    label.verticalCenter = "middle";
    label.fontSize = 40;
  },
};
</script>

<style lang="scss" scoped>
.hello {
  width: 100%;
  height: 300px;
}
</style>