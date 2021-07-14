<template>
  <div class="ml-auto md:ml-0">
    <!-- hamburger menu -->
    <div class="md:hidden ml-auto">
      <svg
        class="w-6 h-6"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16M4 18h16"
        ></path>
      </svg>
    </div>
    <!-- nav -->
    <nav class="space-x-4 text-sm font-medium flex-1 hidden md:flex">
      <a class="bg-gray-800 rounded-lg py-2 px-3 hover:bg-gray-800" href="#"
        >Mailbox</a
      >
      <a class="hover:bg-gray-800 rounded-lg py-2 px-3" href="#">Customers</a>
      <a class="hover:bg-gray-800 rounded-lg py-2 px-3" href="#">Reporting</a>
      <a class="hover:bg-gray-800 rounded-lg py-2 px-3" href="#">Manage</a>
    </nav>
  </div>
</template>
