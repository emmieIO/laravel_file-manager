<template lang="">
    <nav class="min-w-[200px]">
        <div >
            <Link :href="route('myFiles')" class="h-[80px] px-3 flex items-center gap-3">
                <ApplicationLogo
                    class="block h-9 w-auto fill-current text-gray-800"
                />
                <p className="text-2xl">Laradrive</p>
            </Link>
        </div>
        <div className="px-3">
            <CreateNewDropdown />
            <nav class="py-3">
                <NavLink :href="route('myFiles')" :active="$page.url === '/myFiles'">My Files</NavLink>
                <NavLink href="/">Files shared with me</NavLink>
                <NavLink href="/">Files shared by me</NavLink>
                <NavLink href="/">Trash</NavLink>
            </nav>
        </div>
    </nav>
</template>
<script setup>
import { Link } from "@inertiajs/vue3";
import ApplicationLogo from "@/Components/ApplicationLogo.vue";
import CreateNewDropdown from "@/Components/App/CreateNewDropdown.vue";
import NavLink from "../NavLink.vue";
</script>
<style lang=""></style>
