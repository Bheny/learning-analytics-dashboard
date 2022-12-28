<template>
  <div class="p-4 pb-24">
    <div class="w-full mb-4">
        <h2 class="text-2xl font-bold text-slate-800 float-left inline-block w-1/2">My Schedules</h2>
        <button class="rounded-lg p-3 text-white bg-blue-600 float-right inline ">Create Schedule</button>
    </div>
    <div clsas="mt-4">
      <div class="w-full">
        <div
          v-for="schedule in 7"
          v-bind:key="schedule"
          class="mt-3 border rounded-xl p-2 w-full flex"
        >
          <img src="~/assets/ella.jpg" class="rounded-lg w-12 h-12 mr-4" />
          <div class="w-full">
            <div class="md:mr-8 w-full">
              <h2 class="text-sm font-bold text-slate-900">Lesson 4 Test</h2>
              <h3 class="flex text-xs text-slate-400">
                Data Science |
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                  class="w-5 h-5"
                >
                  <path
                    fill-rule="evenodd"
                    d="M5.75 2a.75.75 0 01.75.75V4h7V2.75a.75.75 0 011.5 0V4h.25A2.75 2.75 0 0118 6.75v8.5A2.75 2.75 0 0115.25 18H4.75A2.75 2.75 0 012 15.25v-8.5A2.75 2.75 0 014.75 4H5V2.75A.75.75 0 015.75 2zm-1 5.5c-.69 0-1.25.56-1.25 1.25v6.5c0 .69.56 1.25 1.25 1.25h10.5c.69 0 1.25-.56 1.25-1.25v-6.5c0-.69-.56-1.25-1.25-1.25H4.75z"
                    clip-rule="evenodd"
                  />
                </svg>
                2 days left
              </h3>
            </div>
          </div>
          <div class="">
            <div class="border rounded-lg p-2">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M8.25 4.5l7.5 7.5-7.5 7.5"
                />
              </svg>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
