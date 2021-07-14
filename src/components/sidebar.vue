
<template>
  <div
    class="
      hidden
      w-64
      bg-gray-100
      py-6
      px-4
      overflow-auto
      flex-shrink-0
      lg:block
    "
  >
    <nav class="">
      <!-- mailboxes -->
      <h2 class="font-semibold text-xs text-gray-400 uppercase tracking-wide">
        Mailboxes
      </h2>
      <!-- sidebar items -->
      <div class="space-y-2 mt-6">
        <!--  inbox  -->
        <div
          class="text-sm font-medium text-gray-900 rounded-lg bg-gray-200 -mx-3"
        >
          <a class="flex flex-row items-center p-2" href="#"
            ><svg
              class="w-6 h-6 text-gray-700 flex-shrink-0"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M20 13V6a2 2 0 00-2-2H6a2 2 0 00-2 2v7m16 0v5a2 2 0 01-2 2H6a2 2 0 01-2-2v-5m16 0h-2.586a1 1 0 00-.707.293l-2.414 2.414a1 1 0 01-.707.293h-3.172a1 1 0 01-.707-.293l-2.414-2.414A1 1 0 006.586 13H4"
              ></path>
            </svg>
            <span class="flex-1 ml-2">Inbox</span>
            <span class="flex-shrink-0 bg-gray-300 rounded-full px-3">6</span>
          </a>
        </div>
        <!--  -->
        <!--  flagged  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-700
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center p-2" href="#"
            ><svg
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
                d="M3 21v-4m0 0V5a2 2 0 012-2h6.5l1 1H21l-3 6 3 6h-8.5l-1-1H5a2 2 0 00-2 2zm9-13.5V9"
              ></path>
            </svg>
            <span class="flex-1 ml-2">Flagged</span>
          </a>
        </div>
        <!--  -->
        <!--  Drafts  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-700
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center p-2" href="#"
            ><svg
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
                d="M11 5H6a2 2 0 00-2 2v11a2 2 0 002 2h11a2 2 0 002-2v-5m-1.414-9.414a2 2 0 112.828 2.828L11.828 15H9v-2.828l8.586-8.586z"
              ></path>
            </svg>
            <span class="flex-1 ml-2">Drafts</span>
            <span class="flex-shrink-0 bg-gray-300 rounded-full px-3">2</span>
          </a>
        </div>
        <!--  -->
        <!--  Assigned  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-700
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center p-2" href="#"
            ><svg
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
                d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z"
              ></path>
            </svg>
            <span class="flex-1 ml-2">Assigned</span>
            <span class="flex-shrink-0 bg-gray-300 rounded-full px-3">3</span>
          </a>
        </div>
        <!--  -->
        <!--  Junk  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-700
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center p-2" href="#"
            ><svg
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
                d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4"
              ></path>
            </svg>
            <span class="flex-1 ml-2">Junk</span>
          </a>
        </div>
        <!--  -->
      </div>
      <!-- Folders -->
      <h2
        class="mt-6 font-semibold text-xs text-gray-400 uppercase tracking-wide"
      >
        Folders
      </h2>
      <!--  -->
      <div class="space-y-2 mt-4">
        <!--  Refunds  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-900
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center px-3 py-2" href="#"> Refunds </a>
        </div>
        <!--  -->
        <!--  Discounts  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-900
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center px-3 py-2" href="#">
            Discounts
          </a>
        </div>
        <!--  -->
        <!--  Bugs  -->
        <div
          class="
            text-sm
            font-medium
            text-gray-900
            rounded-lg
            hover:bg-gray-200
            -mx-3
          "
        >
          <a class="flex flex-row items-center px-3 py-2" href="#"> Bugs </a>
        </div>
        <!--  -->
      </div>
    </nav>
  </div>
</template>
