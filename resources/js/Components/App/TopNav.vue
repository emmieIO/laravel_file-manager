<template>
  <fwb-navbar class="w-full sm:flex-row flex-col flex items-center justify-between p-5 " solid>
       <SearchFrom/>
        <UserSettingsDropdown/>
  </fwb-navbar>
</template>

<script setup>
import SearchFrom from "@/Components/App/SearchForm.vue";
import UserSettingsDropdown from "@/Components/App/UserSettingsDropdown.vue"
</script>