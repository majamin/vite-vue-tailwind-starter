<script setup lang="ts">
const data = {
  header: ["model", "mpg", "hp", "gear"],
  values: [
    ["Mazda RX4", 21.0, 110, 4],
    ["Mazda RX4 Wag", 21.0, "NA", 4],
    ["Datsun 710", 22.8, 93, 4],
    ["Hornet 4 Drive", 21.4, 110, 3],
    ["Valiant", 18.1, 105, 3],
  ],
};
</script>
<template>
  <div class="relative overflow-x-auto">
    <table>
      <thead>
        <tr>
          <th v-for="heading in data.header" scope="col">
            {{ heading }}
          </th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="row in data.values">
          <th scope="row">{{ row[0] }}</th>
          <td>{{ row[1] }}</td>
          <td>{{ row[2] }}</td>
          <td>{{ row[3] }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style scoped lang="postcss">
table {
  @apply w-full text-left text-sm text-gray-500 dark:text-gray-400;
}
thead {
  @apply text-xs uppercase border-b-4 text-gray-700 dark:bg-gray-700 dark:text-gray-400;
}
thead > tr > th {
  @apply py-3 px-6;
}
tbody > tr {
  @apply border-b bg-white dark:border-gray-700 dark:bg-gray-800;
}
tbody > tr > th {
  @apply whitespace-nowrap py-4 px-6 font-medium text-gray-900 dark:text-white;
}
tbody > tr > td {
  @apply py-4 px-6;
}
</style>
