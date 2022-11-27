<template>
    <div>
      <div>
        <h1 class="text-xl font-bold">Hello Adam,</h1>
        <h3 class="text-sm text-slate-800 ">Its sunny today and a good time to study</h3>
      </div>
      <div class="mt-4">
        <h2 class="font-bold text-xl">Your Progress <span class="p-2 rounded-full bg-slate-400 text-black text-xs">10</span></h2>
      </div>
      <div class="mt-4">
        <div class="rounded-lg p-3 slate-gray-50 w-64 shadow-lg">
            <div class="p-2">
              <h1 class=" font-bold"><span class="text-2xl">204/</span><span class="text-xl text-slate-400">300</span></h1>
              <h2 class="text-xs text-slate-400">completed Lessons</h2>
            </div>
            <div class="w-full mt-6 mb-6">
              <span class="text-3xl font-bold">65%</span><br />
              <span class="text-xs text-slate-400">completed</span><br />
              <div class="w-full border border-gray-400 bg-white h-2 rounded-full">
                <div class="bg-gray-400 w-1/2 h-full"></div>
              </div>
            </div>
        </div>
      </div>
      <div class="mt-4 pt-4 w-full">
        <div class="mt-4 flex gap-4">
          <div class="w-1/2">
            <h2 class="font-bold text-xl w-full">Activity <span class="p-2 rounded-full bg-slate-400 text-black text-xs">3</span>
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 float-right">
                <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 6h9.75M10.5 6a1.5 1.5 0 11-3 0m3 0a1.5 1.5 0 10-3 0M3.75 6H7.5m3 12h9.75m-9.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-3.75 0H7.5m9-6h3.75m-3.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-9.75 0h9.75" />
              </svg>

            </h2>
            <div class="mx-auto p-3 rounded-lg">
              <div class="flex p-4 border-gray-300 rounded-lg bg-gray-100"><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="mr-3 w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
              </svg>
              <input type="search" />
            </div>
            <ActivityCard />
            </div>
           
          </div>
          <div class="w-1/2">
            <h2 class="font-bold text-xl w-full">Courses <span class="p-2 rounded-full bg-slate-400 text-black text-xs">3</span>
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 float-right">
                <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 6h9.75M10.5 6a1.5 1.5 0 11-3 0m3 0a1.5 1.5 0 10-3 0M3.75 6H7.5m3 12h9.75m-9.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-3.75 0H7.5m9-6h3.75m-3.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-9.75 0h9.75" />
              </svg>

            </h2>
            <div class="mx-auto p-3 rounded-lg">
              <div class="flex p-4 border-gray-300 rounded-lg bg-gray-100"><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="mr-3 w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
              </svg>
              <input type="search" />
            </div>
            <CourseCard />
            </div>
           
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>

  </script> 