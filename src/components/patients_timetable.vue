<template>
  <div class="border border-gray-300 rounded p-5 m-5 h-80">
    <div class="mb-4 border-b border-gray-400">
      <ul
        class="flex flex-wrap -mb-px justify-end"
        id="myTab"
        data-tabs-toggle="#myTabContent"
        role="tablist"
      >
        <div
          class="datepicker relative form-floating mb-3 xl:w-96"
          data-mdb-toggle-button="false"
        >
          <input
            type="text"
            class="
              form-control
              block
              w-1/2
              px-3
              py-1.5
              text-base
              font-normal
              text-gray-700
              bg-white bg-clip-padding
              border border-solid border-gray-300
              rounded
              transition
              ease-in-out
              m-0
              focus:text-gray-700
              focus:bg-white
              focus:border-blue-600
              focus:outline-none
            "
            placeholder="Select a date"
            data-mdb-toggle="datepicker"
          />
        </div>
        <li class="mr-2" role="presentation">
          <button
            class="
              inline-block
              py-4
              px-4
              text-sm
              font-medium
              text-center text-gray-500
              rounded-t-lg
              border-b-2 border-transparent
              hover:text-gray-600 hover:border-gray-300
            "
            id="profile-tab"
            data-tabs-target="#profile"
            type="button"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
          >
            Day
          </button>
        </li>
        <li class="mr-2" role="presentation">
          <button
            class="
              inline-block
              py-4
              px-4
              text-sm
              font-medium
              text-center text-gray-500
              rounded-t-lg
              border-b-2 border-transparent
              hover:text-gray-600 hover:border-gray-300
              active
            "
            id="dashboard-tab"
            data-tabs-target="#dashboard"
            type="button"
            role="tab"
            aria-controls="dashboard"
            aria-selected="true"
          >
            Week
          </button>
        </li>
        <li class="mr-2" role="presentation">
          <button
            class="
              inline-block
              py-4
              px-4
              text-sm
              font-medium
              text-center text-gray-500
              rounded-t-lg
              border-b-2 border-transparent
              hover:text-gray-600 hover:border-gray-300
            "
            id="settings-tab"
            data-tabs-target="#settings"
            type="button"
            role="tab"
            aria-controls="settings"
            aria-selected="false"
          >
            Month
          </button>
        </li>
      </ul>
    </div>
    <div id="myTabContent">
      <div
        class="hidden p-4 bg-gray-50 rounded-lg"
        id="profile"
        role="tabpanel"
        aria-labelledby="profile-tab"
      >
        <p class="text-sm text-gray-500">
          This is some placeholder content the
          <strong class="font-medium text-gray-800"
            >Profile tab's associated content</strong
          >. Clicking another tab will toggle the visibility of this one for the
          next. The tab JavaScript swaps classes to control the content
          visibility and styling.
        </p>
      </div>
      <div
        class="p-4 bg-gray-50 rounded-lg"
        id="dashboard"
        role="tabpanel"
        aria-labelledby="dashboard-tab"
      >
        <p class="text-sm text-gray-500">
          This is some placeholder content the
          <strong class="font-medium text-gray-800"
            >Dashboard tab's associated content</strong
          >. Clicking another tab will toggle the visibility of this one for the
          next. The tab JavaScript swaps classes to control the content
          visibility and styling.
        </p>
      </div>
      <div
        class="hidden p-4 bg-gray-50 rounded-lg"
        id="settings"
        role="tabpanel"
        aria-labelledby="settings-tab"
      >
        <p class="text-sm text-gray-500">
          This is some placeholder content the
          <strong class="font-medium text-gray-800"
            >Settings tab's associated content</strong
          >. Clicking another tab will toggle the visibility of this one for the
          next. The tab JavaScript swaps classes to control the content
          visibility and styling.
        </p>
      </div>
      <div
        class="hidden p-4 bg-gray-50 rounded-lg"
        id="contacts"
        role="tabpanel"
        aria-labelledby="contacts-tab"
      >
        <p class="text-sm text-gray-500">
          This is some placeholder content the
          <strong class="font-medium text-gray-800"
            >Contacts tab's associated content</strong
          >. Clicking another tab will toggle the visibility of this one for the
          next. The tab JavaScript swaps classes to control the content
          visibility and styling.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
</style>