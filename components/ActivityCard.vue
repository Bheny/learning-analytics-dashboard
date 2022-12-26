<template>
    <div>
        <div v-for="activity in activities" v-bind:key="activity" class="p-2 w-full flex">
            <img src="~/assets/ella.jpg" class="rounded-lg w-12 h-12 mr-4"/>
            <div class="w-full">
                <div class="md:mr-8 w-full">
                <h2 class="text-sm">Mr Sackey</h2>
                <h3 class="text-xs">Database, ER </h3>
            </div>
            <div class="md:mr-8 w-full">
                <h2 class="text-sm">Jan 12:30</h2>
                <h3 class="text-xs">Added a new assignment </h3>
            </div>
            </div>
            <div class="">
                <div class="border rounded-lg p-2">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
</svg>

                </div>

            </div>
        </div>
    </div>
  </template>
  
  <script setup>
    const { activities } = defineProps(['activities']) 
  </script>