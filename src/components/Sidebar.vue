<template>
    <aside
        class="sidebar bg-black/20 rounded-3xl backdrop-blur-md shadow-lg ring-1 ring-black/5 p-4"
    >
        <ul class="space-y-4">
            <li>
                <a href="#" class="block text-white hover:text-gray-400">
                    Home
                </a>
            </li>
            <li>
                <a href="#" class="block text-white hover:text-gray-400">
                    My Files
                </a>
            </li>
            <li>
                <a href="#" class="block text-white hover:text-gray-400">
                    Shared
                </a>
            </li>
            <li>
                <a href="#" class="block text-white hover:text-gray-400">
                    Trash
                </a>
            </li>
            <li>
                <a href="#" class="block text-white hover:text-gray-400">
                    Settings
                </a>
            </li>
        </ul>
    </aside>
</template>

<script>
export default {
    name: "Sidebar",
};
</script>

<style scoped>
.sidebar {
    width: 250px;
    min-height: 100vh;
}
</style>
