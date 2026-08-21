<template>
    <header class="bg-[#0B0B10E0] py-6 grid-container border-b border-[#FFFFFF12]">
        <nav class="flex items-center justify-between text-base">
            <NuxtLink to="/" class="flex items-center gap-2">
                <Icon class="text-4xl text-[#6d56e8]" name="tabler:square-letter-a-filled"/>
                <span class="text-[14px] leading-[100%] tracking-wide font-semibold uppercase">Apex</span>
            </NuxtLink>
            <div class="flex items-center gap-4 text-[#7e7c96]">
                <NuxtLink to="/" class="transition-all duration-300 hover:text-[#edeaf5]">Как работает</NuxtLink>
                <NuxtLink to="/" class="transition-all duration-300 hover:text-[#edeaf5]">Возможности</NuxtLink>
                <NuxtLink to="/" class="bg-[#6d56e8] text-white px-4 py-2 rounded-md transition-all duration-300 font-semibold hover:-translate-y-px hover:bg-[#8570f5]">Начать</NuxtLink>
            </div>
        </nav>
    </header>
</template>

<script setup>

</script>