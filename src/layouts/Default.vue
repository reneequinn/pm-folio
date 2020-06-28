<template>
  <div class="bg-gray-100 flex flex-col min-h-screen antialiased">
    <header class="px-4 py-6 shadow bg-white">
      <div
        class="container mx-auto flex flex-wrap items-center justify-between"
      >
        <h1
          class="font-bold text-xl border-b-2 border-transparent hover:border-indigo-700 transition ease-in duration-200"
        >
          <g-link to="/">Project Management Folio</g-link>
        </h1>
        <div class="block lg:hidden">
          <button
            @click="toggle"
            class="flex items-center justify-center fill-current text-black p-1 rounded border-2 border-black hover:text-indigo-700 hover:border-indigo-700 transition ease-in duration-200"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              height="24"
              viewBox="0 0 24 24"
              width="24"
            >
              <path d="M0 0h24v24H0V0z" fill="none" />
              <path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z" />
            </svg>
          </button>
        </div>
        <nav
          :class="isOpen ? 'block' : 'hidden'"
          class="w-full flex-grow lg:flex lg:items-center lg:w-auto"
        >
          <ul class="lg:flex items-center text-center ml-auto">
            <li
              class="font-semibold border-b-2 border-transparent hover:border-indigo-700 transition ease-in duration-200 my-3 lg:my-0 lg:mr-8"
            >
              <g-link to="/">Home</g-link>
            </li>
            <li
              class="font-semibold border-b-2 border-transparent hover:border-indigo-700 transition ease-in duration-200 my-3 lg:my-0 lg:mr-8"
            >
              <g-link to="/#about">About</g-link>
            </li>
            <li
              class="font-semibold border-b-2 border-transparent hover:border-indigo-700 transition ease-in duration-200 my-3 lg:my-0"
            >
              <g-link to="/#videos">Videos</g-link>
            </li>
          </ul>
        </nav>
      </div>
    </header>
    <main class="flex-grow px-4">
      <slot />
    </main>
    <footer class="bg-white px-4 py-4 shadow">
      <div class="container mx-auto text-center">
        <p>Made with ❤ by Renee Quinn</p>
      </div>
    </footer>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>
