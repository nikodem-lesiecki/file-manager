<template>
    <div class="app flex">
        <Sidebar />
        <div class="flex-1">
            <Navbar />
        </div>
    </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";

export default {
    components: {
        Navbar,
        Sidebar,
    },
};
</script>

<style scoped>
.app {
    display: flex;
    gap: 15px;
}
</style>
