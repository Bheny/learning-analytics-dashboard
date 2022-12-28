<!-- <template>
    <div>
      <canvas ref="pieChart" width="400" height="400"></canvas>
    </div>
  </template>
  
  <script>
  import { Pie, mixins } from 'vue-chartjs/nuxt'
  
  export default {
    extends: Pie,
    // mixins: [mixins.reactiveProp],
    props: ['chartData', 'options'],
    mounted () {
      this.renderChart(this.chartData, this.options)
    }
  }
  </script>
  
 -->





<!-- <template>
    <Pie :data="chartData" :options="chartOptions" />
  </template>
  
  <script >
  import { Chart as ChartJS, ArcElement, Tooltip, Legend } from 'chart.js'
  import { Pie } from 'vue-chartjs'
 
  
  ChartJS.register(ArcElement, Tooltip, Legend)
  
  export default {
    name: 'PieChart',
    components: {
      Pie
    },
    props: {
      
      chartData: {
        type: Object,
        default: () => {}
      },
      chartOptions: {
      type: Object,
      default: () => {}
    }
    },
  }
  </script> -->