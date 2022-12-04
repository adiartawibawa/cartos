<template>
    <div class="min-h-full">

        <Navbars />

        <header class="bg-white shadow" v-if="$slots.header">
            <div class="mx-auto max-w-7xl py-6 px-4 sm:px-6 lg:px-8">
                <h1 class="text-3xl font-bold tracking-tight text-gray-900">
                    <slot name="header" />
                </h1>
            </div>
        </header>

        <main>
            <slot />
        </main>

    </div>
</template>

<script setup>
import Navbars from '@/Components/Navbars.vue';
</script>