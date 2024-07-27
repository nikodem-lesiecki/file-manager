<template>
    <nav
        class="bg-black/20 rounded-3xl backdrop-blur-md shadow-lg ring-1 ring-black/5"
    >
        <div
            class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
        >
            <div class="search-bar relative">
                <label for="Search" class="sr-only">Search</label>
                <input
                    type="text"
                    id="Search"
                    placeholder="Search for..."
                    class="focus:outline:none text-white bg-transparent w-full rounded-md border-none py-2.5 pr-10 shadow-sm sm:text-sm"
                />
                <span
                    class="absolute inset-y-0 right-0 grid w-10 place-content-center"
                >
                    <button
                        type="button"
                        class="text-gray-600 hover:text-gray-700"
                    >
                        <span class="sr-only">Search</span>
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            stroke="currentColor"
                            class="h-4 w-4"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
                            />
                        </svg>
                    </button>
                </span>
            </div>
            <div class="upload">
                <a
                    class="group inline-block rounded-full bg-gradient-to-r from-blue-600 to-violet-600 p-[2px] hover:text-white focus:outline-none focus:ring active:text-opacity-75"
                    href="#"
                >
                    <span
                        class="block rounded-full bg-white/20 px-8 py-3 text-sm font-medium group-hover:bg-transparent"
                    >
                        Upload
                    </span>
                </a>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: "Navbar",
};
</script>

<style scoped>
.search-bar {
    width: 50rem;
}
</style>
