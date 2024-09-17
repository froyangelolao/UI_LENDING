<template>
    <div class="px-4 sm:px-6 lg:px-8">
        <div class="sm:flex sm:items-center">
            <div class="sm:flex-auto">
                <h1 class="text-base font-bold leading-6 text-gray-900">Dashboard Libraries Roles</h1>
                <p class="mt-2 text-sm text-gray-700">A list of all the users in your account including their name, title,
                    email, and role.</p>
            </div>
            <div class="mt-4 sm:ml-16 sm:mt-0 sm:flex-none">
                <button type="button"
                    class="block rounded-md bg-indigo-600 px-3 py-2 text-center text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Add
                    user</button>
            </div>
        </div>
        <div class="mt-6 flow-root shadow-sm border rounded-lg overflow-x-auto">
            <div class="-mx-4 -my-2 overflow-x-auto sm:-mx-6 lg:-mx-8">
                <div class="inline-block min-w-full py-2 align-middle sm:px-6 lg:px-8">
                    <table class="w-full table-auto text-sm text-left">
                        <thead class="bg-gray-50 text-gray-600 font-medium border-b">
                            <tr>
                                <th scope="col"
                                    class="py-3.5 pl-4 pr-3 text-left text-sm font-semibold text-whtie sm:pl-3">Name</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-whtie">City</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-whtie">Province</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-whtie">Country</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-whtie">Name Type</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-whtie">Actions</th>
                            </tr>
                        </thead>
                        <tbody class="bg-white">
                            <template v-for="location in locations" :key="location.name">
                                <tr class="border-t border-gray-200">
                                    <th colspan="5" scope="colgroup"
                                        class="bg-gray-50 py-2 pl-4 pr-3 text-left text-sm font-semibold text-gray-900 sm:pl-3">
                                        {{ location.name }}</th>
                                </tr>
                                <tr v-for="(person, personIdx) in location.people" :key="person.name"
                                    :class="[personIdx === 0 ? 'border-gray-300' : 'border-gray-200', 'border-t']">
                                    <td class="whitespace-nowrap py-6 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-3">
                                        {{ person.name }}</td>
                                    <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">{{ person.city }}</td>
                                    <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">{{ person.province }}</td>
                                    <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">{{ person.country }}</td>
                                    <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">{{ person.nametype }}</td>
                                    <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">
                                        <a href="#" class="text-indigo-600 hover:text-indigo-900 mr-4">Add Form</a>
                                        <a href="#" class="text-indigo-600 hover:text-indigo-900 mr-4">View Form</a>
                                        <a href="#" class="text-indigo-600 hover:text-indigo-900 mr-4">Update</a>
                                        <a href="#" class="text-indigo-600 hover:text-indigo-900">Delete</a>
                                    </td>
                                </tr>
                            </template>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const locations = [
    {
        name: 'Edinburgh',
        people: [
            { name: 'Lindsay Walton', city: 'Davao', province: 'Davao Del Sur', country: 'Philippines', nametype: 'User' },
            { name: 'Lindsay Walton', city: 'Davao', province: 'Davao Del Sur', country: 'Philippines', nametype: 'User' },
            { name: 'Lindsay Walton', city: 'Davao', province: 'Davao Del Sur', country: 'Philippines', nametype: 'User' },
            { name: 'Lindsay Walton', city: 'Davao', province: 'Davao Del Sur', country: 'Philippines', nametype: 'User' },
            { name: 'Lindsay Walton', city: 'Davao', province: 'Davao Del Sur', country: 'Philippines', nametype: 'User' },

        ],
    },
]
</script>
