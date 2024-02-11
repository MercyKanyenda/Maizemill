<template>
    <div class="chart-container">
        <Bar :data="data" :options="options" />
    </div>
  </template>
  
  <script lang="ts">
  import {
    Chart as ChartJS,
    Title,
    Tooltip,
    Legend,
    BarElement,
    CategoryScale,
    LinearScale
  } from 'chart.js'
  import { Bar } from 'vue-chartjs'
  import * as chartConfig from './chartConfig.js'
  
  ChartJS.register(CategoryScale, LinearScale, BarElement, Title, Tooltip, Legend)
  
  export default {
    name: 'App',
    components: {
      Bar
    },
    data() {
      return chartConfig
    }
  }
  </script>

<style>
.chart-container {
  width: 500px; /* Set the desired width */
  height: 300px; /* Set the desired height */
}
</style>
  