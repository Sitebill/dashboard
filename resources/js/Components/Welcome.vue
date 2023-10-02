<script setup>
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import Rating from 'primevue/rating';
import { ref } from 'vue';

const value = ref(null);

</script>

<template>
    <div>
        <div class="p-6 lg:p-8 bg-white border-b border-gray-200">
            <ApplicationLogo class="block h-12 w-auto" />

            <h1 class="mt-8 text-2xl font-medium text-gray-900">
                Welcome to your Jetstream application!
            </h1>
        </div>

        <div class="bg-gray-200 bg-opacity-25 grid grid-cols-1 md:grid-cols-2 gap-6 lg:gap-8 p-6 lg:p-8">
            <div class="card flex justify-content-center">
                <Rating v-model="value" />
            </div>
        </div>
    </div>
</template>
