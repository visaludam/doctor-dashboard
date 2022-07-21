<template>
  <div>
    <div
      class="
        text-4xl
        font-meduim
        text-black
        items-start
        justify-start
        flex
        p-10
        pt-16
      "
    >
      Good {{ time }} Mario
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {};
  },
  data() {
    return {
      time: "",
    };
  },
  mounted() {
    console.log("hshdh");
    const time = new Date().getHours();
    if (time < 12) {
      this.time = "Morning";
    } else if (time >= 12 && time < 17) {
      this.time = "Afternoon";
    } else {
      this.time = "Evening";
    }
  },
};
</script>

<style lang="scss" scoped>
</style>