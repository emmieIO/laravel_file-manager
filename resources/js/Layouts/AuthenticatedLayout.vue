<template>
    <div class="h-screen bg-gray-50 flex w-full gap-4">
        <Navigation/>
        <main class="flex flex-col flex-1 px-4 overflow-hidden">
            <div class="flex items-center justify-between w-full">
                <TopNav/>
            </div>
            <div class="flex-1 flex flex-col overflow-none">
                <slot/>
            </div>
        </main>
    </div>


</template>

<script setup>
import TopNav from "@/Components/App/TopNav.vue"
import Navigation from "@/Components/App/Navigation.vue"
import SearchFrom from "@/Components/App/SearchForm.vue";
import UserSettingsDropdown from "@/Components/App/UserSettingsDropdown.vue"



</script>