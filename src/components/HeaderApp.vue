<template>
  <header class="header shadow-md main-navbar main-navbar__group py-1">
    <nav class="bg-white py-2 md:py-4">
      <div class="container px-md-0 mx-auto md:flex md:items-center">
        <div class="flex justify-between items-center">
          <a href="#" class="font-bold text-xl text-indigo-600">OLA</a>
          <a href="#" class="p-4">Bài viết mới</a>
          <a href="#" class="p-4">Hỏi đáp </a>
          <a href="#" class="p-4">Thảo luận </a>
        </div>

        <div
          class="hidden md:flex flex-col md:flex-row md:ml-auto mt-3 md:mt-0"
          id="navbar-collapse"
        >
          <div class="relative">
            <input
              type="text"
              placeholder="Tìm kiếm..."
              class="border rounded-lg px-4 py-2 w-64 focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
            <button
              class="absolute right-0 top-0 px-3 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-500"
            >
              Tìm kiếm
            </button>
          </div>
          <a
            href="#"
            class="p-2 lg:px-4 md:mx-2 text-indigo-600 text-center border border-solid border-indigo-600 rounded hover:bg-indigo-100 hover:text-indigo-700 transition-colors duration-300"
            >Đăng nhập</a
          >
          <a
            href="#"
            class="p-2 lg:px-4 md:mx-2 text-indigo-600 text-center border border-solid border-indigo-600 rounded hover:bg-indigo-600 hover:text-white transition-colors duration-300 mt-1 md:mt-0 md:ml-1"
            >Đăng kí</a
          >
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderApp",
};
</script>

<style scoped></style>
