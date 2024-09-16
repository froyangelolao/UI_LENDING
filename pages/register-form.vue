<template>
    <div class="min-h-screen flex items-center justify-center">
      <div class="flex w-full max-w-5x1 bg-white shadow-lg">
        <div class="w-1/2 relative">
          <img
            alt="People working in an office"
            class="w-full h-full object-cover"
            src="../img/register-image.png"
          />
          <div class="absolute inset-0 bg-black opacity-50"></div>
          <div class="absolute inset-0 flex flex-col justify-center items-start p-10 text-white">
            <h1 class="text-4xl font-bold">Small Loans, Big Impact</h1>
            <p class="mt-4 text-lg">
              Microfinance provides small loans and financial services to individuals and small businesses in underserved communities, empowering them to achieve financial independence and improve their quality of life.
            </p>
          </div>
        </div>
        <div class="w-1/2 bg-gray-800 p-10">
          <div class="flex justify-center mb-6">
            <img alt="LendCash Logo" class="h-20 w-20" src="../img/LendCash_Logo-removebg-preview.png" />
          </div>
          <h2 class="text-3xl font-bold text-white text-center mb-4">REGISTRATION</h2>
          <h3 class="text-xl font-semibold text-white mb-2">
            Step 1
            <span class="font-normal">| Basic Information</span>
          </h3>
          <p class="text-white mb-6">
            This is a Pre-Registration. To become a fully verified member, we require our dear clients to send their requirements onsite. This includes any type of valid IDs, barangay clearance, PSA, and any type of proof of income.
          </p>
          <form class="space-y-4">
            <div class="flex space-x-4">
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Last Name"
                type="text"
              />
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter First Name"
                type="text"
              />
            </div>
            <div class="flex space-x-4">
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Middle Name"
                type="text"
              />
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Birth Date"
                type="date"
              />
            </div>
            <div class="flex space-x-4">
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Civil Status"
                type="text"
              />
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Birth Place"
                type="text"
              />
            </div>
            <div class="flex space-x-4">
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Gender"
                type="text"
              />
              <input
                class="w-1/2 p-3 rounded-full bg-white text-gray-800"
                placeholder="Enter Date Registered"
                type="date"
              />
            </div>
            <div class="flex justify-between mt-6">
              <button
                class="px-6 py-3 rounded-full bg-purple-600 text-white"
                type="button"
                
              >
              <a href="/"> Cancel</a>
              </button>
              <button class="px-6 py-3 rounded-full bg-purple-600 text-white" type="button">
                
                <a href="register-submitted">Next </a>
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
    <footer class="absolute bottom-0 w-full text-center py-4 bg-white text-gray-800">
      2024 LendCash. All Rights Reserved.
    </footer>
  </template>
  
  <script>
  export default {
    head: {
      title: 'Register',
      link: [
        {
          rel: 'stylesheet',
          href: 'https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap',
        },
      ],
    },
  }
  </script>
  
  <style>
  body {
    font-family: 'Roboto', sans-serif;
  }
  </style>