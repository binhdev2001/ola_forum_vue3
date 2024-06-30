<template>
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Template Bami App</title>
    </head>
    <body>
      <div id="root">
        <div class="content-wrapper text-base mx-auto bg-gray-100">
          <nav
            class="navbar header-background flex px-20 justify-between py-1 bg-primary-yellow"
          >
            <div class="nav-left p-0 flex text-center items-center gap-10">
              <div class="logo p-0">
                <img
                  class="w-32 object-cover"
                  src="/images/bami_logo.svg"
                  alt=""
                />
              </div>
              <div
                class="search-box flex items-center px-4 rounded-3xl bg-white"
              >
                <Icon icon="mdi:search" class="text-gray-500 text-2xl" />
                <input
                  type="text"
                  placeholder="Search"
                  class="border-0 focus:outline-none p-2 w-60"
                />
              </div>
            </div>

            <div class="nav-right p-0 flex items-center gap-3">
              <ul
                class="navicon flex justify-center gap-2 text-black text-5xl flex"
              >
                <li class="">
                  <a href="#"><Icon class="w-6" icon="mdi:email" /></a>
                </li>
                <li>
                  <a href="#"><Icon class="w-6" icon="mdi:notifications" /></a>
                </li>
              </ul>
              <div class="profile-image online" onclick="">
                <img
                  class="rounded-full object-cover w-10 h-10"
                  src="images/profile-pic.png"
                  alt=""
                />
              </div>
            </div>
            <div
              class="user-settings hidden absolute right-8 top-14 max-w-80 w-full bg-white shadow-xl"
            >
              <div class="profile-darkButton flex items-center py-5">
                <div class="user-profile flex items-center w-3/5">
                  <img
                    class="rounded-full object-cover w-10 h-10"
                    src="images/profile-pic.png"
                    alt=""
                  />
                  <div class="box-profile px-4 text-gray-600">
                    <p class="font-semibold text-xl p-0">Phương Bình</p>
                    <a class="" href="#">Xem chi tiết</a>
                  </div>
                </div>
                <div class="flex w-2/5 items-center justify-center">
                  <label
                    for="dark-mode-toggle"
                    class="flex items-center cursor-pointer w-11"
                  >
                    <div class="relative">
                      <input
                        type="checkbox"
                        id="dark-mode-toggle"
                        class="sr-only"
                        onchange=""
                      />
                      <div
                        class="block bg-gray-600 w-14 h-8 rounded-full"
                      ></div>
                      <div
                        class="dot absolute left-1 top-1 bg-white w-6 h-6 rounded-full transition"
                      ></div>
                    </div>
                  </label>
                </div>
              </div>
              <hr />
              <div class="logout-links flex items-center justify-between pt-8">
                <div class="flex items-center justify-between gap-5">
                  <Icon class="w-9 h-9 ml-2" icon="mdi:logout" />
                  <a class="" href="#">Logout</a>
                </div>
                <Icon icon="mdi:navigate-next" />
              </div>
            </div>
          </nav>
          <main class="px-20 mt-2">
            <section class="flex gap-3 justify-between">
              <div class="sidebar-left w-1/4">
                <div class="important-links">
                  <div class="border-b-2">
                    <a
                      class="flex items-center justify-start gap-5 text-2xl mb-8"
                      href="#"
                    >
                      <Icon
                        class="text-3xl text-blue-600"
                        icon="mdi:newspaper"
                      />
                      Latest news
                    </a>
                    <a
                      class="flex items-center justify-start gap-5 text-2xl mb-8"
                      href="#"
                    >
                      <Icon
                        class="text-3xl text-blue-600"
                        icon="mdi:user-multiple"
                      />
                      Friends
                    </a>
                    <a
                      class="flex items-center justify-start gap-5 text-2xl mb-8 bo"
                      href="#"
                    >
                      <Icon
                        class="text-3xl text-blue-600"
                        icon="mdi:user-multiple"
                      />
                      Marketplace
                    </a>
                  </div>
                  <div class="shortcut-links">
                    <h2 class="font-semibold text-2xl mb-5">Chủ đề</h2>
                    <a
                      class="flex items-center justify-start gap-5 text-xl mb-8"
                      href="#"
                    >
                      <img
                        class="w-10"
                        src="images/shortcut-1.png"
                        alt=""
                      />Công nghệ thông tin
                    </a>
                    <a
                      class="flex items-center justify-start gap-5 text-xl mb-8"
                      href="#"
                    >
                      <img class="w-10" src="images/shortcut-2.png" alt="" />Tin
                      tức - sự kiện
                    </a>
                    <a
                      class="flex items-center justify-start gap-5 text-xl mb-8"
                      href="#"
                    >
                      <img
                        class="w-10"
                        src="images/shortcut-3.png"
                        alt=""
                      />Tuyển dụng việc làm
                    </a>
                  </div>
                </div>
              </div>
              <div class="last-news w-1/2 bg-yellow-500">new post content</div>
              <div class="sidebar-right w-1/4 bg-red-600">sidebar right</div>
            </section>
          </main>
        </div>
      </div>
    </body>
  </html>
</template>
<style>
.header-background {
  background-color: #f9dfaf;
  background-image: url("/public/images/Header-Background.jpg");
  background-blend-mode: soft-light;
  transform: rotate(0deg);
}
</style>
<script>
import { Icon } from "@iconify/vue";
export default {
  components: {
    Icon,
  },
  name: "Template",
  props: {
    msg: String,
  },
};
</script>
