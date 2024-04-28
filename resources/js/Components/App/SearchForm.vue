<template lang="">
    <div class="w-full sm:w-[50%] ">
        <form class="">
        <TextInput 
        type="text" 
        class="block w-full"
        placeholder="Search for files and folder" autocomplete
        v-model="form.search" 
        />
        </form>
    </div>
</template>
<script setup>
import { useForm } from '@inertiajs/vue3';
import TextInput from '../TextInput.vue';


//Uses
const form = useForm({
    search : ""
})
</script>
<style lang="">
</style>