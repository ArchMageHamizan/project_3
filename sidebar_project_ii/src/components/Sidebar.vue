<template>
    <div class="relative flex min-h-screen">
        <!-- ====================== sidebar ================== -->
        <div :class="{'relative -translate-x-0': showSidebarButton, '-translate-x-full': !showSidebarButton}" class="bg-green-600 text-cyan-100 w-64 space-y-6 px-2 absolute inset-y-0 left-0 transform transition duration-200 ease-in-out">
            <a href="" class="flex items-center justify-center py-4 gap-2 ">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-10 w-10">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m21 7.5-2.25-1.313M21 7.5v2.25m0-2.25-2.25 1.313M3 7.5l2.25-1.313M3 7.5l2.25 1.313M3 7.5v2.25m9 3 2.25-1.313M12 12.75l-2.25-1.313M12 12.75V15m0 6.75 2.25-1.313M12 21.75V19.5m0 2.25-2.25-1.313m0-16.875L12 2.25l2.25 1.313M21 14.25v2.25l-2.25 1.313m-13.5 0L3 16.5v-2.25" />
                </svg>
                <span class="text-2xl font-extrabold text-white">Hamizan Yusni</span>
            </a>
            <nav>
                <a href="/" class="flex items-center space-x-2 px-6 py-2 hover:bg-green-500 hover:text-yellow-300 group rounded transition duration-200">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
                    </svg>
                    <span class="text-white group-hover:text-yellow-300">About Me</span>
                </a>
                <a href="/" class="flex items-center space-x-2 px-6 py-2 hover:bg-green-500 rounded hover:text-yellow-300 group transition duration-200">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 14.25v-2.625a3.375 3.375 0 0 0-3.375-3.375h-1.5A1.125 1.125 0 0 1 13.5 7.125v-1.5a3.375 3.375 0 0 0-3.375-3.375H8.25m0 12.75h7.5m-7.5 3H12M10.5 2.25H5.625c-.621 0-1.125.504-1.125 1.125v17.25c0 .621.504 1.125 1.125 1.125h12.75c.621 0 1.125-.504 1.125-1.125V11.25a9 9 0 0 0-9-9Z" />
                    </svg>
                    <span class="text-white group-hover:text-yellow-300">Projects</span>
                </a>
                <a href="/" class="flex items-center space-x-2 px-6 py-2 hover:bg-green-500 rounded hover:text-yellow-300 group transition duration-200">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M12 21a9.004 9.004 0 0 0 8.716-6.747M12 21a9.004 9.004 0 0 1-8.716-6.747M12 21c2.485 0 4.5-4.03 4.5-9S14.485 3 12 3m0 18c-2.485 0-4.5-4.03-4.5-9S9.515 3 12 3m0 0a8.997 8.997 0 0 1 7.843 4.582M12 3a8.997 8.997 0 0 0-7.843 4.582m15.686 0A11.953 11.953 0 0 1 12 10.5c-2.998 0-5.74-1.1-7.843-2.918m15.686 0A8.959 8.959 0 0 1 21 12c0 .778-.099 1.533-.284 2.253m0 0A17.919 17.919 0 0 1 12 16.5c-3.162 0-6.133-.815-8.716-2.247m0 0A9.015 9.015 0 0 1 3 12c0-1.605.42-3.113 1.157-4.418" />
                    </svg>
                    <span class="text-white group-hover:text-yellow-300">Experience</span>
                </a>
                <a href="/" class="flex items-center space-x-2 px-6 py-2 hover:bg-green-500 rounded hover:text-yellow-300 group transition duration-200">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 0 0 2.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 0 1-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 0 0-1.091-.852H4.5A2.25 2.25 0 0 0 2.25 4.5v2.25Z" />
                    </svg>
                    <span class="text-white group-hover:text-yellow-300">Contact</span>
                </a>
            </nav>
        </div>
        <!-- ====================== main content ============= -->
        <div class="flex-1">
            <div class="bg-white shadow px-2 py-4">
                <button class="text-green-600 font-extrabold" @click="toggleSidebar">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-8 w-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                    </svg>
                </button>
            </div>
            <div class="p-8 text-green-700 font-extrabold">content</div>
            <div class="px-2 py-4">footer</div>
        </div>
    </div>
</template>

<script>
import { ref, onMounted } from 'vue';

export default {
    setup() {
        const showSidebarButton = ref(true);

        const toggleSidebar = () => {
            showSidebarButton.value = !showSidebarButton.value;
            localStorage.setItem('sidebarState', showSidebarButton.value);
        };

        onMounted(() => {
            const savedState = localStorage.getItem('sidebarState');
            if (savedState !== null) {
                showSidebarButton.value = JSON.parse(savedState);
            }
        });

        return {
            showSidebarButton,
            toggleSidebar
        };
    }
};
</script>

<style scoped>
/* Add any additional styling you need here */
</style>
