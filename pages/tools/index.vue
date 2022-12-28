<template>
  <div class="p-4">
    <h2 class="text-2xl font-bold text-slate-800">Tools</h2>
  </div>
  <div class="p-2 pb-24">
    <!-- Mentor finder -->
    <div
      class=" flex shadow-lg to-bg-blue-300 bg-gradient-to-r from-blue-500 rounded-xl p-3"
    >
      <div class="text-white">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-16 h-16 mt-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M15 19.128a9.38 9.38 0 002.625.372 9.337 9.337 0 004.121-.952 4.125 4.125 0 00-7.533-2.493M15 19.128v-.003c0-1.113-.285-2.16-.786-3.07M15 19.128v.106A12.318 12.318 0 018.624 21c-2.331 0-4.512-.645-6.374-1.766l-.001-.109a6.375 6.375 0 0111.964-3.07M12 6.375a3.375 3.375 0 11-6.75 0 3.375 3.375 0 016.75 0zm8.25 2.25a2.625 2.625 0 11-5.25 0 2.625 2.625 0 015.25 0z"
          />
        </svg>
      </div>
      <div>
        <h2 class="text-2xl font-bold text-slate-900">Find me a Mentor..</h2>
        <p class="text-sm">
          Connect with alumni and other strong candidates in your field of study
          for mentorship sessions
        </p>
        <button
          class="rounded-lg text-white to-blue-600 bg-gradient-to-r from-blue-800 p-3 w-full mx-auto text-center mt-2"
        >
          Get Started
        </button>
      </div>
    </div>

    <!-- Job finder -->
    <div
      class="mt-3 flex shadow-lg  bg-gradient-to-r from-red-500 to-bg-red-300 rounded-xl p-3"
    >
      <div class="text-white">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-16 h-16 mt-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M20.25 14.15v4.25c0 1.094-.787 2.036-1.872 2.18-2.087.277-4.216.42-6.378.42s-4.291-.143-6.378-.42c-1.085-.144-1.872-1.086-1.872-2.18v-4.25m16.5 0a2.18 2.18 0 00.75-1.661V8.706c0-1.081-.768-2.015-1.837-2.175a48.114 48.114 0 00-3.413-.387m4.5 8.006c-.194.165-.42.295-.673.38A23.978 23.978 0 0112 15.75c-2.648 0-5.195-.429-7.577-1.22a2.016 2.016 0 01-.673-.38m0 0A2.18 2.18 0 013 12.489V8.706c0-1.081.768-2.015 1.837-2.175a48.111 48.111 0 013.413-.387m7.5 0V5.25A2.25 2.25 0 0013.5 3h-3a2.25 2.25 0 00-2.25 2.25v.894m7.5 0a48.667 48.667 0 00-7.5 0M12 12.75h.008v.008H12v-.008z"
          />
        </svg>
      </div>
      <div>
        <h2 class="text-2xl font-bold text-slate-900">Find me a Job..</h2>
        <p class="text-sm">
          Check out all the jobs under a fields to know your prospects as a
          student
        </p>
        <button
          class="rounded-lg text-white bg-gradient-to-r from-red-500 to-red-400 p-3 w-full mx-auto text-center mt-2"
        >
          Get Started
        </button>
      </div>
    </div>

    <!-- My Counseller -->
    <div
      class="mt-3 flex shadow-lg  bg-gradient-to-r from-blue-500 to-bg-blue-300 rounded-xl p-3"
    >
      <div class="text-white">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-16 h-16 mt-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M9 12.75L11.25 15 15 9.75m-3-7.036A11.959 11.959 0 013.598 6 11.99 11.99 0 003 9.749c0 5.592 3.824 10.29 9 11.623 5.176-1.332 9-6.03 9-11.622 0-1.31-.21-2.571-.598-3.751h-.152c-3.196 0-6.1-1.248-8.25-3.285z"
          />
        </svg>
      </div>
      <div>
        <h2 class="text-2xl font-bold text-slate-900">Counsellor..</h2>
        <p class="text-sm">
          Find out the relevancy of any topic or activity in the course you are
          taking ..
        </p>
        <button
          class="rounded-lg text-white to-blue-600 bg-gradient-to-r from-blue-800 p-3 w-full mx-auto text-center mt-2"
        >
          Get Started
        </button>
      </div>
    </div>
    <div
      class="mt-3 flex shadow-lg  bg-gradient-to-r from-red-500 to-bg-red-300 rounded-xl p-3"
    >
      <div class="text-white">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-16 h-16 mt-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75a4.5 4.5 0 01-4.884 4.484c-1.076-.091-2.264.071-2.95.904l-7.152 8.684a2.548 2.548 0 11-3.586-3.586l8.684-7.152c.833-.686.995-1.874.904-2.95a4.5 4.5 0 016.336-4.486l-3.276 3.276a3.004 3.004 0 002.25 2.25l3.276-3.276c.256.565.398 1.192.398 1.852z" />
  <path stroke-linecap="round" stroke-linejoin="round" d="M4.867 19.125h.008v.008h-.008v-.008z" />
</svg>

        
      </div>
      <div>
        <h2 class="text-2xl font-bold text-slate-900">Tricks & Hacks..</h2>
        <p class="text-sm">
          Did you know the shortcuts in the course you are studying that will make studying easier for you ?
        </p>
        <button
          class="font-bold rounded-lg text-white bg-gradient-to-r from-red-500 to-red-400 p-3 w-full mx-auto text-center mt-2"
        >
          Get Started
        </button>
      </div>
    </div>
  </div>
</template>
