<!-- hide the footer from "cover" layout -->
<template>
    <footer
      v-if="$nav.currentLayout !== 'cover'"
      class="absolute bottom-0 left-0 right-0 p-2 text-xs  c-blue-gray-5 italic" 
    >
      Data Analytics. Author: Geoff Matheson, Heathmont College, 2025
    </footer>
  </template>