<template>
  <div class="relative overflow-x-auto shadow-md sm:rounded-lg">
    <table class="w-full text-sm text-left text-gray-500 dark:text-gray-400">
      <thead
        class="
          text-xs text-gray-700
          uppercase
          bg-gray-50
          dark:bg-gray-700 dark:text-gray-400
        "
      >
        <tr>
          <th scope="col" class="px-6 py-3">رقم المنتج</th>
          <th scope="col" class="px-6 py-3"> صورة المنتج </th>
          <th scope="col" class="px-6 py-3">اسم المنتج</th>
          <th scope="col" class="px-6 py-3"> سعر المنتج</th>
          <th scope="col" class="px-6 py-3">الحاله</th>
          <th scope="col" class="px-6 py-3">
            <span class="sr-only">Edit</span>
          </th>
          <th scope="col" class="px-6 py-3">
            <span class="sr-only">Delete</span>
          </th>
        </tr>
      </thead>
      <tbody>
        <tr class="bg-white border-b dark:bg-gray-800 dark:border-gray-700" :key="item" v-for="item in 5">
          <th
            scope="row"
            class="
              px-6
              py-4
              font-medium
              text-gray-900
              dark:text-white
              whitespace-nowrap
            "
          >
            1
          </th>
          <td class="px-6 py-4">
              <img src="https://images.ulta.com/is/image/Ulta/2588402" alt="" class="w-20">
          </td>
          <td class="px-6 py-4">منتج تجريبي</td>
          <td class="px-6 py-4">199.999$ </td>
          <td class="px-6 py-4">
           متوفر
          </td>
            <td class="px-6 py-4">
              <router-link to="/EditProduct">
                 <a
              href="#"
              class="
                font-medium
                text-blue-600
                dark:text-blue-500
                hover:underline
              "
              >تعديل </a
            >
              </router-link>
                
          </td>
          <td class="px-6 py-4">
                 <a
              href="#"
              class="
                font-medium
                text-red-600
                dark:text-blue-500
                hover:underline
              "
              >حذف </a
            >
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
    name:"OrdersTable"
};
</script>

<style>
</style>