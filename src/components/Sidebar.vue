<!-- Sidebar.vue -->
<template>
    <aside
        class="sidebar bg-black/20 rounded-3xl backdrop-blur-md shadow-lg ring-1 ring-black/5 p-4"
    >
        <ul class="space-y-4">
            <template v-for="file in fs" :key="file.name">
                <li @click="selectFile(file)" class="cursor-pointer">
                    <a class="block text-white hover:text-gray-400">{{
                        file.name
                    }}</a>
                </li>
                <ul v-if="file.directory" class="ml-4 space-y-2">
                    <li
                        v-for="subFile in file.directory"
                        :key="subFile.name"
                        @click.stop="selectFile(subFile)"
                        class="cursor-pointer"
                    >
                        <a class="block text-white hover:text-gray-400">{{
                            subFile.name
                        }}</a>
                    </li>
                </ul>
            </template>
        </ul>
    </aside>
</template>

<script>
export default {
    name: "Sidebar",
    data() {
        return {
            fs: [
                {
                    name: "main.js",
                    content: "console.log('hello')",
                },
                {
                    name: "index.html",
                    content: "<html></html>",
                },
                {
                    name: "components",
                    directory: [
                        {
                            name: "button.js",
                            content:
                                "export function Button() { return <button>test</button> }",
                        },
                        {
                            name: "table",
                            directory: [{ name: "table.js", content: "" }],
                        },
                        {
                            name: "subdir",
                            directory: [
                                {
                                    name: "haha.txt",
                                    content: "haha lol",
                                },
                            ],
                        },
                    ],
                },
            ],
        };
    },
    methods: {
        selectFile(file) {
            this.$emit("file-selected", file);
        },
    },
};
</script>

<style scoped>
.sidebar {
    width: 250px;
    min-height: 100vh;
}
</style>
