<template>
  <q-page class="q-pa-sm">
    <div class="row q-col-gutter-sm q-py-sm">
      <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
        <bar-chart></bar-chart>
      </div>
      <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
        <line-chart></line-chart>
      </div>
      <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
        <scatter-plot></scatter-plot>
      </div>
      <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
        <pie-chart></pie-chart>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent, defineAsyncComponent } from "vue";
import "echarts";
export default defineComponent({
  name: "charts",
  components: {
    PieChart: defineAsyncComponent(() => import("components/charts/PieChart")),
    ScatterPlot: defineAsyncComponent(() =>
      import("components/charts/ScatterPlot")
    ),
    LineChart: defineAsyncComponent(() =>
      import("components/charts/LineChart")
    ),
    BarChart: defineAsyncComponent(() => import("components/charts/BarChart")),
  },
});
</script>
<style scoped></style>
