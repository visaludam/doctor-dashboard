<template>
  <div class="border border-gray-300 rounded p-5 m-5 h-96 overflow-y-auto">
    <div class="flex justify-start">
      <div class="font-medium">Contacts</div>
    </div>
    <div
      class="
        flex
        items-center
        my-3
        p-3
        rounded-md
        justify-between
        hover:bg-gray-100
      "
      v-for="con in contacts"
      :key="con.index"
    >
      <div class="group flex items-center">
        <img
          class="
            shrink-0
            inline-block
            h-12
            w-12
            rounded-full
            ring-1 ring-gray-300
          "
          src="../assets/profile/ally.png"
        />
        <!-- :src="require(`../assets/profile/${con.img}`)" -->

        <div class="px-4">
          <div class="text-md font-medium">{{ con.name }}</div>
          <span class="text-sm font-normal hover:font-medium">{{
            con.position
          }}</span>
        </div>
      </div>
      <div class="p-2 border border-gray-200 rounded-md">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4 text-gray-500"
          viewBox="0 0 20 20"
          fill="currentColor"
        >
          <path
            d="M6 10a2 2 0 11-4 0 2 2 0 014 0zM12 10a2 2 0 11-4 0 2 2 0 014 0zM16 12a2 2 0 100-4 2 2 0 000 4z"
          />
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      contacts: [
        {
          name: "Liam Miller",
          position: "Oncologist",
          img: "liam.png",
        },
        {
          name: "Fiona Smith",
          position: "Head of the clinic",
          img: "fiona.png",
        },
        {
          name: "Mike Bailey",
          position: "Diagnostics",
          img: "mike.png",
        },
        {
          name: "Charlie Backham",
          position: "Neurosurgeon",
          img: "liam.png",
        },
        {
          name: "Ally Jack",
          position: "Neurologist",
          img: "chalie.png",
        },
        { name: "Olga Zack", position: "Diagnostics" },
        { name: "Victor Quinn", position: "Neurosurgeon" },
      ],
    };
  },
  setup() {
    return {};
  },
};
</script>

<style>
</style>