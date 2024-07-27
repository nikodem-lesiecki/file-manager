<template>
    <div
        class="file-viewer bg-black/20 rounded-3xl backdrop-blur-md shadow-lg ring-1 ring-black/5 p-4 flex justify-center items-center"
    >
        <div class="text-white">No file selected</div>
    </div>
</template>

<script>
export default {
    name: "FileViewer",
};
</script>

<style>
.file-viewer {
    margin-top: 15px;
}
</style>
