<template>
    <div id="profileSection" class="rounded-lg mt-4 md:mt-0 bg-gray-100 lg:w-2/6 p-6">
        <div class="mb-6 p-2">
            <h2 class="text-lg font-bold inline-block text-gray-700">Profile</h2>
        <button class="bg-gray-400 text-gray-700 p-2 rounded-lg float-right">Edit</button>
        </div>
        <div class="mt-6 text-center">
            <img src="../assets/ella.jpg" class="mx-auto object-center border border-4 border-blue-600 object-cover rounded-full h-24 w-24" />
            <h2 class="font-bold mt-2 text-gray-900 text-lg">{{ user.firstname }} {{user.lastname}}</h2>
            <h3 class="text-gray-600 text-sm">@{{ user.username}}</h3>
        </div>
        <div class="mt-4">
            <div class="grid grid-cols-3 text-center bg-gray-200 rounded-lg ">
                <div  class="p-2">
                    <h3 class="text-gray-600 text-xs">Rank</h3>
                    <h2 class="font-bold text-sm text-gray-900">12</h2>
                </div>
                <div  class="p-2">
                    <h3 class="text-gray-600 text-xs">Average Act.</h3>
                    <h2 class="font-bold text-sm text-gray-900">2,300</h2>
                </div>
                <div  class="p-2">
                    <h3 class="text-gray-600 text-xs">Courses</h3>
                    <h2 class="font-bold text-sm text-gray-900">6</h2>
                </div>
            </div>
        </div>
        <div>
            <h2 class="font-bold text-gray-700 mt-4 p-2">My Badges</h2>
            <div class="grid grid-cols-3 ">
                <div v-for="badge in 6" :key="badge" class="p-3">
                    <img src="~/assets/ella.jpg" class="mx-auto object-center border border-4 border-blue-600 object-cover rounded-full h-16 w-16" />
                </div>
            </div>
        </div>
        <h2 class="font-bold text-gray-700 mt-4 p-2">Calender</h2>
        <!-- <CalenderModule /> -->
        <h2 class="font-bold text-gray-700 mt-4 p-2">Up coming Classes</h2>
        <div class="overflow-y-scroll h-64">
            <div v-for="course in courses" :key="course.id" class="hover:border-blue-600 hover:bg-blue-100 hover:text-gray-100 hover:border-4 border rounded-lg mt-2 flex bg-white p-3"><input type="checkbox" class="mt-1 h-2 bg-blue-600 text-white mr-2 inline-block rounded-lg w-4 h-4 float-left"/><div class="text-gray-900 text-sm inline-block font-bold text-center">{{ course.title }}<br><span class="text-gray-500 text-xs">{{ course.date }} from {{ course.start}} to {{ course.end }}</span></div><svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-gray-600 float-right inline-block" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
  <path stroke-linecap="round" stroke-linejoin="round" d="M4 8V4m0 0h4M4 4l5 5m11-1V4m0 0h-4m4 0l-5 5M4 16v4m0 0h4m-4 0l5-5m11 5l-5-5m5 5v-4m0 4h-4" />
</svg></div>
        </div>
    
        
            
        
    </div>
</template>

<script setup>
const user = ref( {
        id:1,
        username:"0321080183",
        firstname:"Adam",
        lastname: "Taylor",
        email:"adam.taylor@htu.edu.gh",
        is_student:true,
        class:"Btech Computer Science 300",
      })

      const courses = ref([
            {id:1,title:'Software Architecture',date:'May 2, 2020', start:'8:00 Am', end:'10:00 AM'},
            {id:1,title:'Computer Literacy',date:'May 3, 2020', start:'8:00 Am', end:'10:00 AM'},
            {id:1,title:'MIS',date:'May 4, 2020', start:'8:00 Am', end:'10:00 AM'},
            ])

</script>