<template>
  <div  id="BarChart" class="p-3 pb-24">
    <div>
      <h2 class="text-2xl font-bold">Analytics</h2>
      <h3>April 30, Thursday</h3>
    </div>
    <div class="grid lg:grid-cols-3 gap-4 lg:w-3/5 w-full mt-3">
      <div class="rounded-lg border flex p-4">
        <div class="mr-3 bg-blue-800 rounded-full w-16 h-16 text-center">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
            stroke="currentColor" class="mx-auto text-white w-6 mt-4 h-6">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M3 13.125C3 12.504 3.504 12 4.125 12h2.25c.621 0 1.125.504 1.125 1.125v6.75C7.5 20.496 6.996 21 6.375 21h-2.25A1.125 1.125 0 013 19.875v-6.75zM9.75 8.625c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125v11.25c0 .621-.504 1.125-1.125 1.125h-2.25a1.125 1.125 0 01-1.125-1.125V8.625zM16.5 4.125c0-.621.504-1.125 1.125-1.125h2.25C20.496 3 21 3.504 21 4.125v15.75c0 .621-.504 1.125-1.125 1.125h-2.25a1.125 1.125 0 01-1.125-1.125V4.125z" />
          </svg>

        </div>
        <div>
          <h2 class="text-slate-400 text-xs">overall Engagement</h2>
          <h1 class="text-slate-400"><span class="text-2xl text-black font-bold">18h/</span>weekly</h1>
        </div>
      </div>
      <div class="rounded-lg border flex p-4">
        <div class="mr-3 bg-blue-800 rounded-full w-16 h-16 text-center">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
            stroke="currentColor" class="mx-auto text-white w-6 mt-4 h-6">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M11.48 3.499a.562.562 0 011.04 0l2.125 5.111a.563.563 0 00.475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 00-.182.557l1.285 5.385a.562.562 0 01-.84.61l-4.725-2.885a.563.563 0 00-.586 0L6.982 20.54a.562.562 0 01-.84-.61l1.285-5.386a.562.562 0 00-.182-.557l-4.204-3.602a.563.563 0 01.321-.988l5.518-.442a.563.563 0 00.475-.345L11.48 3.5z" />
          </svg>


        </div>
        <div>
          <h2 class="text-slate-400 text-xs">Points Scored</h2>
          <h1 class="text-slate-400"><span class="text-2xl text-black font-bold">600/</span>6000</h1>
        </div>
      </div>
      <div class="rounded-lg border flex p-4">
        <div class="mr-3 bg-blue-800 rounded-full w-16 h-16 text-center">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
            stroke="currentColor" class="mx-auto text-white w-6 mt-4 h-6">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M15 19.128a9.38 9.38 0 002.625.372 9.337 9.337 0 004.121-.952 4.125 4.125 0 00-7.533-2.493M15 19.128v-.003c0-1.113-.285-2.16-.786-3.07M15 19.128v.106A12.318 12.318 0 018.624 21c-2.331 0-4.512-.645-6.374-1.766l-.001-.109a6.375 6.375 0 0111.964-3.07M12 6.375a3.375 3.375 0 11-6.75 0 3.375 3.375 0 016.75 0zm8.25 2.25a2.625 2.625 0 11-5.25 0 2.625 2.625 0 015.25 0z" />
          </svg>


        </div>
        <div>
          <h2 class="text-slate-400 text-xs">Your Rank</h2>
          <h1 class="text-slate-400"><span class="text-2xl text-black font-bold">135/</span>200</h1>
        </div>
      </div>
    </div>
    <div >
      <BarChart :chartData="barChartData" :chartOptions="barChartOptions" />

      <!-- <PieChart :chartData="pieChartData" :chartOptions="pieChartOptions" /> -->

   
  </div>
  </div>
  
</template>
  
<script setup>
const barChartData = {
        labels: [ 'January', 'February', 'March' ],
        datasets: [ { label: 'Database',
                  backgroundColor: '#1152d3',
                      data: [40, 20, 12] },{ label: 'Data Analytics',
                  backgroundColor: '#f87923',
                      data: [20, 70, 45] } ]
      }
const barChartOptions = ref( {
        responsive: true
      })

//       const pieChartData = {
//           labels: ['VueJs', 'EmberJs', 'ReactJs', 'AngularJs'],
//           datasets: [
//     {
//       backgroundColor: ['#41B883', '#E46651', '#00D8FF', '#DD1B16'],
//       data: [40, 20, 30, 10]
//     }
//   ]
// }
// const pieChartOptions = {
//   responsive: true,
//   maintainAspectRatio: false
// }
</script>

<!-- <script>
import { Bar, Bubble } from 'vue-chartjs'
import { Chart as ChartJS, Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale } from 'chart.js'

ChartJS.register(Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale)

export default {
  name: 'BarChart',
  components: { Bar, Bubble },
  data() {
    return {
      chartData: {
        labels: [ 'January', 'February', 'March' ],
        datasets: [ { label: 'Database',
                  backgroundColor: '#1152d3',
                      data: [40, 20, 12] },{ label: 'Data Analytics',
                  backgroundColor: '#f87923',
                      data: [20, 70, 45] } ]
      },
      chartOptions: {
        responsive: true
      }
    }
  }
}
</script> -->
