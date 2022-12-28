<template>
    <Bar
      :options="chartOptions"
      :data="chartData"
      
    />
  </template>
  
  <script>
  import { Bar } from 'vue-chartjs'
  import { Chart as ChartJS, Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale } from 'chart.js'
  
  ChartJS.register(Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale)
  
  export default {
    name: 'BarChart',
    components: { Bar },
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
    // d@agbeko#*
    //  data() {
    //   return {
    //     // chartData: {
    //     //   labels: [ 'January','Febuary','March','April','May','June','July','August','September','October','November','December'],
    //     //   datasets: [ { data: [40, 20, 12, 34, 56, 67, 21, 55, 33, 12, 67, 33] } ]
    //     // },
    //     // chartOptions: {
    //     //   responsive: true
    //     // },
    //     // styles: ['bg-blue-600'],
    //   }
    // }
//     data() {
//     return {
//       chartData: {
//         labels: [ 'January', 'February', 'March' ],
//         datasets: [ { label: 'Database',
//                   backgroundColor: '#1152d3',
//                       data: [40, 20, 12] },{ label: 'Data Analytics',
//                   backgroundColor: '#f87923',
//                       data: [20, 70, 45] } ]
//       },
//       chartOptions: {
//         responsive: true
//       }
//     }
//   }
  }
  </script>