<template>
  <div class="relative mt-1">
    <div
      class="
        flex
        absolute
        inset-y-0
        left-0
        items-center
        pl-3
        pointer-events-none
      "
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-5 w-5 text-gray-400"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
        />
      </svg>
    </div>
    <input
      type="text"
      id="text-input"
      class="
        bg-white
        border border-gray-300
        text-gray-900 text-sm
        rounded-full
        focus:ring-blue-500 focus:border-blue-500
        block
        w-full
        pl-10
        p-2.5
        dark:bg-gray-700
        dark:border-gray-600
        dark:placeholder-gray-400
        dark:text-white
        dark:focus:ring-blue-500
        dark:focus:border-blue-500
      "
      placeholder="Search appointment, patients, etc"
    />
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
</style>