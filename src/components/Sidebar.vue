<template>
  <nav class="bg-secondMain w-80 z-1000 right-0 md:w-72 h-screen md:h-auto md:block absolute md:static" :class="{ block: isMenuOpen, hidden: !isMenuOpen }">
    <div class="max-w-7xl mx-auto py-3 md:py-4">
      <div class="flex items-center justify-center">
        <div class="items-center w-full hidden md:flex flex-col">

            <div class="flex justify-start py-6 px-8 w-full flex items-center ">
              <svg class="text-blue-500 md:h-9 md:w-9 md:inline hidden pr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
              </svg>
            <div class="font-semibold text-white">Recruiter</div>
            </div>
            <ul class="flex flex-col w-full">
              <li class="py-3 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent active">
                <a href="#" class="px-4 font-medium flex jystify-start items-center pl-8">
                  <svg class="md:h-9 md:w-9 md:inline hidden pr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 012-2h2a2 2 0 012 2m0 10a2 2 0 002 2h2a2 2 0 002-2M9 7a2 2 0 012-2h2a2 2 0 012 2m0 10V7m0 10a2 2 0 002 2h2a2 2 0 002-2V7a2 2 0 00-2-2h-2a2 2 0 00-2 2" />
                  </svg>
                  <span class="text-gray-400 font-bold">Dashboard</span>
                </a>
              </li>
              <li class=" py-3 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
                <a href="#" class="px-4 font-medium flex jystify-start items-center pl-8">
                  <svg class="md:h-9 md:w-9 md:inline hidden pr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                  </svg>
                  <span class="text-gray-400 font-bold">Jobs</span>
                </a>
              </li>
              <li class=" py-3 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
                <a href="#" class="px-4 font-medium flex jystify-start items-center pl-8">
                  <svg class="md:h-9 md:w-9 md:inline hidden pr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21h10a2 2 0 002-2V9.414a1 1 0 00-.293-.707l-5.414-5.414A1 1 0 0012.586 3H7a2 2 0 00-2 2v14a2 2 0 002 2z" />
                  </svg>
                  <span class="text-gray-400 font-bold">Applications</span>
                </a>
              </li>
              <li class=" py-3 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
                <a href="#" class="px-4 font-medium flex jystify-start items-center pl-8">
                  <svg class="md:h-9 md:w-9 md:inline hidden pr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z" />
                  </svg>
                  <span class="text-gray-400 font-bold">Team</span>
                </a>
              </li>
              <li class=" py-3 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
                <a href="#" class="px-4 font-medium flex jystify-start items-center pl-8">
                  <svg class="md:h-9 md:w-9 md:inline hidden pr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 3.055A9.001 9.001 0 1020.945 13H11V3.055z" />
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.488 9H15V3.512A9.025 9.025 0 0120.488 9z" />
                  </svg>
                  <span class="text-gray-400 font-bold">Reports</span>
                </a>
              </li>
            </ul>
        </div>
      </div>
    </div>

    <!-- Mobile menu, show/hide based on menu state. -->
    <div class="md:hidden" id="mobile-menu">
      <!-- Mobile menu button -->
      <div class="flex justify-end pr-6">
        <button @click="$emit('openMenu')" type="button" class="bg-transparent inline-flex items-center justify-center p-2 text-gray-200 rounded-md hover:text-white hover:bg-gray-700 focus:outline-none" aria-controls="mobile-menu" aria-expanded="false">
          <svg class="block h-8 w-8" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button> 
      </div>
              
      <ul class="flex flex-col items-baseline w-full ">
        <li class="w-full active py-4 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
          <a href="#" class="text-gray-400 px-6 py-2 font-bold">Dashboard</a>
        </li>
        <li class="w-full  py-4 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
          <a href="#" class="text-gray-400 px-6 py-2 font-bold">Jobs</a>
        </li>
        <li class="w-full  py-4 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
          <a href="#" class="text-gray-400 px-6 py-2 font-bold">Applications</a>
        </li>
        <li class="w-full  py-4 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
          <a href="#" class="text-gray-400 px-6 py-2 font-bold">Team</a>
        </li>
        <li class="w-full  py-4 nav-li hover:cursor-pointer border-r-4 border-transparent hover:border-accent">
          <a href="#" class="text-gray-400 px-6 py-2 font-bold">Reports</a>
        </li>
      </ul>
    </div>
<!-- </transition> -->
  </nav>
<!-- </transition> -->
</template>

<script>
export default {
  name: "SideBar",
    data: () => {
    return {
      isUserMenuOpen: false,
    }
  },
  props: {
    isMenuOpen: Boolean
  },
  methods: {
    openUserMenu() {
      this.isUserMenuOpen = !this.isUserMenuOpen
    },

  }
};
</script>

<style scoped>
.nav-li:hover span, .nav-li.active span{
  color: #fff;
}
.nav-li:hover a,.nav-li.active a  {
  color: #3d7eff;
}

.nav-li.active {
  cursor: pointer !important;
  border-right: 4px solid #3d7eff !important;
}
</style>
