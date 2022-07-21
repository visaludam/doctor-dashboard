<template>
  <div class="border border-gray-300 rounded p-5 m-5">
    <div class="flex justify-between">
      <div class="font-medium">Analytics</div>
      <div class="flex items-center">
        <div class="text-sm">This week</div>
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
  mounted() {},
};
</script>

<style lang="scss" scoped>
.hello {
  width: 100%;
  height: 300px;
}
</style>