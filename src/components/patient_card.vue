<template>
  <div class="bg-blue-900 text-white rounded p-5 mx-5">
    <div class="flex justify-between">
      <div>Patients</div>
      <div class="flex items-center">
        <div class="text-sm">This month</div>
        <span class="px-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-3 w-3"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
              clip-rule="evenodd"
            /></svg
        ></span>
      </div>
    </div>
    <div class="flex items-center justify-start">
      <div class="text-5xl font-light">58</div>
      <div class="px-5">
        <div class="text-base font-medium">New patients</div>
        <div class="text-sm text-green-500 font-medium flex">
          <span class="pr-2"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-3 w-3"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M14.707 12.707a1 1 0 01-1.414 0L10 9.414l-3.293 3.293a1 1 0 01-1.414-1.414l4-4a1 1 0 011.414 0l4 4a1 1 0 010 1.414z"
                clip-rule="evenodd"
              /></svg
          ></span>
          68%
        </div>
      </div>
    </div>
    <div class="flex items-center justify-start py-4">
      <div class="text-5xl font-light">72</div>
      <div class="px-5">
        <div class="text-base font-medium">Old patients</div>
        <div class="text-sm text-green-500 font-medium flex">
          <span class="pr-2"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-3 w-3"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M14.707 12.707a1 1 0 01-1.414 0L10 9.414l-3.293 3.293a1 1 0 01-1.414-1.414l4-4a1 1 0 011.414 0l4 4a1 1 0 010 1.414z"
                clip-rule="evenodd"
              /></svg
          ></span>
          83%
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>