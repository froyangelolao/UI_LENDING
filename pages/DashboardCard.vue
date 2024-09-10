<template>
    <div class="w-full md:w-1/2 xl:w-1/4 px-6 py-2">
      <div class="bg-white rounded-lg shadow-md p-5">
        <h4 class="text-lg font-semibold text-gray-700">{{ title }}</h4>
        <div class="flex items-center justify-between mt-4">
          <div class="text-2xl font-bold text-gray-900">{{ value }}</div>
          <button class="bg-blue-500 hover:bg-blue-600 text-white px-4 py-2 rounded">
            View
          </button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    name: 'DashboardCard',
    props: {
      title: {
        type: String,
        required: true,
      },
      value: {
        type: [String, Number],
        required: true,
      },
    },
  });
  </script>