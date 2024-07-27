<template>
    <div class="app flex">
        <Sidebar />
        <div class="flex-1">
            <Navbar />
            <FileViewer />
        </div>
    </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";
import FileViewer from "./components/FileViewer.vue";

export default {
    components: {
        Navbar,
        Sidebar,
        FileViewer,
    },
};
</script>

<style scoped>
.app {
    display: flex;
    gap: 15px;
}
</style>
