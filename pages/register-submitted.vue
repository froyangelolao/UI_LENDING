<template>
    <div class="min-h-screen flex">
      <div class="w-1/2 relative">
        <img
          alt="People working in an office"
          class="absolute inset-0 w-full h-full object-cover"
          src="../img/register-image.png"
        />
        <div class="absolute inset-0 bg-black opacity-50"></div>
        <div class="relative z-10 p-12 text-white">
          <h1 class="text-5xl font-bold text-white">Small Loans, Big Impact</h1>
          <p class="mt-4 text-lg text-white">
            Microfinance provides small loans and financial services to individuals and small businesses in underserved communities, empowering them to achieve financial independence and improve their quality of life.
          </p>
        </div>
      </div>
      <div class="w-1/2 bg-gray-800 flex flex-col justify-between">
        <div class="p-12 text-white">
          <div class="flex justify-center mb-8">
            <img alt="LendCash logo" class="h-20 w-" src="../img/LendCash_Logo-removebg-preview.png" />
          </div>
          <h2 class="text-4xl font-bold text-center mb-4 text-white">REGISTRATION</h2>
          <h3 class="text-2xl font-semibold text-center mb-4 text-white">
            Step 2
            <span class="text-xl text-white">Advance Information</span>
          </h3>
          <p class="text-center mb-8 text-white">
            This is a Pre-Registration. To become a fully verified member, we require our dear clients to send their requirements online. This includes any type of valid IDs, barangay clearance, PSA, and any type of proof of income.
          </p>
          <form class="space-y-4">
            <input
              class="w-full p-3 rounded-full bg-gray-700 text-white"
              placeholder="Enter Phone Number"
              type="text"
            />
            <input
              class="w-full p-3 rounded-full bg-gray-700 text-white"
              placeholder="Enter valid Email"
              type="email"
            />
            <input
              class="w-full p-3 rounded-full bg-gray-700 text-white"
              placeholder="Enter Current Address"
              type="text"
            />
            <input
              class="w-full p-3 rounded-full bg-gray-700 text-white"
              placeholder="Enter Occupation"
              type="text"
            />
            <input
              class="w-full p-3 rounded-full bg-gray-700 text-white"
              placeholder="Enter Co-Borrower"
              type="text"
            />
            <div class="flex justify-between items-center">
              <div class="w-1/2 pr-2">
                <div class="bg-gray-700 p-3 rounded-full text-center text-white">
                  Valid ID Image
                </div>
                <input
                  class="mt-2 w-full"
                  type="file"
                  accept="image/*"
                />
              </div>
              <div class="w-1/2 pl-2">
                <div class="bg-gray-700 p-3 rounded-full text-center text-white">
                  Barangay Clearance Image
                </div>
                <input
                  class="mt-2 w-full"
                  type="file"
                  accept="image/*"
                />
              </div>
            </div>
            <div class="flex justify-between items-center">
              <div class="w-1/2 pr-2">
                <div class="bg-gray-700 p-3 rounded-full text-center text-white">
                  PSA Image
                </div>
                <input
                  class="mt-2 w-full"
                  type="file"
                  accept="image/*"
                />
              </div>
            </div>
          </form>
        </div>
        <div class="flex justify-between p-12">
          <button class="bg-purple-600 text-white px-6 py-3 rounded-full">
            Back
          </button>
          <button class="bg-purple-600 text-white px-6 py-3 rounded-full">
            <a href="register-final">Submit</a>
          </button>
        </div>
        <footer class="bg-gray-900 text-center py-4 text-white">
          <p>2023 LendCash. All Rights Reserved.</p>
        </footer>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    setup() {
      return {}
    }
  }
  </script>