<template>
    <div>
        <div v-for="course in courses" v-bind:key="course" class="p-2 w-full flex">
            <img src="~/assets/ella.jpg" class="rounded-lg w-12 h-12 mr-4"/>
            <div class="mr-24">
                <h2 class="text-sm text-slate-600 font-bold">Introduction to Programming</h2>
                <h3 class="text-xs text-slate-400">By Mr Asiedu </h3>
                <div>
                    <h4 class="text-sm text-slate-500">Course 112</h4>
                </div>
            </div>
        </div>
    </div>
  </template>
  
  <script setup>
    const { courses } = defineProps(['courses'])
  </script>