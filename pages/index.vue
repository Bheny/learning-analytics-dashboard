<template>
    <div class="p-3 pb-24">
      <div class="">
        <h1 class="text-2xl text-slate-800 font-bold">Hello Adam,</h1>
        <h3 class="text-sm text-slate-800 ">Its sunny today and a good time to study</h3>
      </div>
      <div class="mt-4">
        <h2 class="font-bold text-xl">Your Progress <span class="p-2 rounded-full bg-blue-800 text-white text-xs">10</span></h2>
      </div>
      <div class="mt-4 md:flex md:gap-3">
        <!-- lessons completed card -->
        <div class="rounded-lg p-3 slate-gray-50 md:w-64 shadow-lg">
            <div class="p-2">
              <h1 class=" font-bold"><span class="text-slate-800 text-2xl">204/</span><span class="text-xl text-slate-400">300</span></h1>
              <h2 class="text-xs text-slate-400">completed Lessons</h2>
            </div>
            <div class="w-full mt-6 mb-6">
              <span class="text-3xl text-slate-800 font-bold">65%</span><br />
              <span class="text-xs text-slate-400">completed</span><br />
              <div class="w-full border border-gray-400 bg-white h-2 rounded-full">
                <div class="bg-blue-500 w-1/2 h-full"></div>
              </div>
            </div>
        </div>
        <!-- overall ranking -->
        <div class="rounded-lg p-3 slate-gray-50 md:w-64 shadow-lg">
            <div class="p-2">
              <h2  class="text-lg text-slate-900 py-4">You Rank at </h2>
              <h1 class=" font-bold"><span class="text-2xl">135/</span><span class="text-xl text-slate-400">200</span></h1>
              <h2 class="text-xs text-slate-400">other students</h2>
            </div>
            <div class="hidden w-full mt-6 mb-6">
              <span class="text-3xl font-bold">65%</span><br />
              <span class="text-xs text-slate-400">completed</span><br />
              <div class="w-full border border-gray-400 bg-white h-2 rounded-full">
                <div class="bg-gray-400 w-1/2 h-full"></div>
              </div>
            </div>
        </div>
      </div>
      <div class="mt-8 ">
        <h2 class="font-bold text-xl md:text-2xl w-full">Recommended For You <span class="text-sm text-blue-600 underline float-right">View More</span></h2>
        <div class="w-full mt-3  lg:flex overflow-x-scroll gap-3">
         <div v-for="recommended in 3" @key="recommended" class="w-full mt-3 inline-block lg:w-full bg-blue-50 rounded-xl">
           <!-- course recommendation : courses or articales are rendered based on the courses student is taking  -->
           <div class="w-full">
            <img src="~/assets/ella.jpg" class="rounded-xl w-full h-48 object-cover object-center" />
          </div>
          <div class="mt-2 p-2">
            <h4 class="text-slate-400 text-xs">Projector | 7 min read</h4>
            <h2 class="font-bold text-slate-900 text-lg">Understanding Databases for beginners</h2>
          </div>
         </div>

        </div>
      </div>
     <div class="mt-4 pt-4 md:w-5/6">
        <div class="mt-4 md:flex md:gap-4">
          <div class="w-full lg:w-1/2">
            <h2 class="font-bold text-xl w-full">Activity <span class="p-2 rounded-full bg-slate-400 text-black text-xs">3</span>
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 float-right">
                <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 6h9.75M10.5 6a1.5 1.5 0 11-3 0m3 0a1.5 1.5 0 10-3 0M3.75 6H7.5m3 12h9.75m-9.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-3.75 0H7.5m9-6h3.75m-3.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-9.75 0h9.75" />
              </svg>

            </h2>
            <div class="mx-auto p-3 rounded-lg">
              <div class="flex p-4 border-gray-300 rounded-lg bg-gray-100"><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="mr-3 w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
              </svg>
              <input type="search" class="w-full"/>
            </div>
            <ActivityCard :activities="5"/>
            </div>
           
          </div>
          <div class="w-full lg:w-1/2">
            <h2 class="font-bold text-xl w-full">Courses <span class="p-2 rounded-full bg-slate-400 text-black text-xs">3</span>
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 float-right">
                <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 6h9.75M10.5 6a1.5 1.5 0 11-3 0m3 0a1.5 1.5 0 10-3 0M3.75 6H7.5m3 12h9.75m-9.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-3.75 0H7.5m9-6h3.75m-3.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-9.75 0h9.75" />
              </svg>

            </h2>
            <div class="mx-auto p-3 rounded-lg">
              <div class="flex p-4 border-gray-300 rounded-lg bg-gray-100"><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="mr-3 w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
              </svg>
              <input type="search"  class="w-full"/>
            </div>
            <CourseCard :courses="5" />
            </div>
           
          </div>
        </div>
      </div> 
      <div class="pt-4 ">
        <h2 class="font-bold text-xl">Community Ranking </h2>
        <div class="overflow-x-scroll mt-8">
          <table class="w-full gap-3 table">
            
            
              <th class="text-lg pr-24">Student</th>
              <th class="text-lg pr-24">Ranking</th>
              <th class="text-lg pr-24">Courses</th>
              <th class="text-lg pr-24">Hours</th>
              <th class="text-lg pr-24">Score</th>
  
            
              <tr v-for="student in 15" @key="student" class="h-16 pt-3 border-b">
                  <td class="pr-24">
                    <!-- student card -->
                    <div class="flex gap-3">
                      <img src="~/assets/ella.jpg" class="w-12 h-12 rounded-full" />
                      <span class="font-bold text-sm">Issac Newton</span>
                    </div>
                  </td>
                  <td class="pr-24">
                    <!-- ranking card -->
                    <span>{{student}}</span>
                    <span>up</span>
                  </td>
                  <td class="pr-24">
                    41
                  </td>
                  <td class="pr-24">
                    30:40
                  </td>
                  <td class="pr-24">
                    <span class="text-green-600 mr-3 text-xs">+65</span>
                    <span>670</span>
                  </td>
              </tr>
          
          </table>
        </div>
      </div>
      <profile />
    </div>
  </template>
  
  <script setup>

  </script> 