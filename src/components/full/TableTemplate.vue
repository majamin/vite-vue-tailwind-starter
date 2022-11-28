<script setup lang="ts">
</script>
<template>
  <div class="relative overflow-x-auto">
    <table class="w-full text-left text-sm text-gray-500 dark:text-gray-400">
      <thead
        class="bg-gray-50 text-xs uppercase text-gray-700 dark:bg-gray-700 dark:text-gray-400"
      >
        <tr>
          <th scope="col" class="py-3 px-6">Product name</th>
          <th scope="col" class="py-3 px-6">Color</th>
          <th scope="col" class="py-3 px-6">Category</th>
          <th scope="col" class="py-3 px-6">Price</th>
        </tr>
      </thead>
      <tbody>
        <tr class="border-b bg-white dark:border-gray-700 dark:bg-gray-800">
          <th
            scope="row"
            class="whitespace-nowrap py-4 px-6 font-medium text-gray-900 dark:text-white"
          >
            Apple MacBook Pro 17"
          </th>
          <td class="py-4 px-6">Sliver</td>
          <td class="py-4 px-6">Laptop</td>
          <td class="py-4 px-6">$2999</td>
        </tr>
        <tr class="border-b bg-white dark:border-gray-700 dark:bg-gray-800">
          <th
            scope="row"
            class="whitespace-nowrap py-4 px-6 font-medium text-gray-900 dark:text-white"
          >
            Microsoft Surface Pro
          </th>
          <td class="py-4 px-6">White</td>
          <td class="py-4 px-6">Laptop PC</td>
          <td class="py-4 px-6">$1999</td>
        </tr>
        <tr class="bg-white dark:bg-gray-800">
          <th
            scope="row"
            class="whitespace-nowrap py-4 px-6 font-medium text-gray-900 dark:text-white"
          >
            Magic Mouse 2
          </th>
          <td class="py-4 px-6">Black</td>
          <td class="py-4 px-6">Accessories</td>
          <td class="py-4 px-6">$99</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
