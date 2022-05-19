<template>
    <!-- Content -->
    <div class="px-3 py-10 md:px-10">
        <div class="w-full sm:w-1/2 lg:w-1/3 mx-auto">

            <!-- Todo spinner -->
            <div class="text-center">
                <img
                    src="@/assets/img/spinner.svg"
                    alt=""
                    class="inline-block w-5 h-5"
                >
            </div>
            <!--/ Todo spinner -->

            <!-- Todo form -->
            <form class="flex items-center px-4 bg-gray-900 h-15
rounded-sm border-l-2 border-green-400 mb-3">
                <input
                    placeholder="Adicione um novo item ..."
                    type="text"
                    class="bg-gray-900 placeholder-gray-500 text-gray-500
font-light focus:outline-none block w-full appearance-none leading-normal
py-3 pr-3"
                >

                <button
                    class="text-green-400 text-xs font-semibold
focus:outline-none"
                    type="submit"
                >
                    ADICIONAR
                </button>
            </form>
            <!--/ Todo form -->

            <!-- Todo items -->
            <div class="space-y-2">
                <div class="bg-gray-300 rounded-sm">
                    <div class="flex items-center px-4 py-3 border-b
border-gray-400 last:border-b-0">
                        <div class="flex items-center justify-center
mr-2">
                            <button class="text-gray-400">
                                <svg class="w-5 h-5" fill="none"
                                     stroke="currentColor" viewBox="0 0 24 24"
                                     xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round"
                                                                              stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            </button>
                        </div>

                        <div class="w-full">
                            <input
                                type="text"
                                placeholder="Digite a sua tarefa"
                                value="Estudar Vue 3"
                                class="bg-gray-300 placeholder-gray-500
text-gray-700 font-light focus:outline-none block w-full appearance-none
leading-normal mr-3"
                            >
                        </div>

                        <div class="ml-auto flex items-center
justify-center">
                            <button class="focus:outline-none">
                                <svg
                                    class="ml-3 h-4 w-4 text-gray-500"
                                    viewBox="0 0 24 24"
                                    fill="none"
                                    stroke="currentColor"
                                    xmlns="http://www.w3.org/2000/svg"
                                >
                                    <path
                                        d="M19 7L18.1327 19.1425C18.0579
20.1891 17.187 21 16.1378 21H7.86224C6.81296 21 5.94208 20.1891 5.86732
19.1425L5 7M10 11V17M14 11V17M15 7V4C15 3.44772 14.5523 3 14 3H10C9.44772
3 9 3.44772 9 4V7M4 7H20"
                                        stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                    />
                                </svg>
                            </button>
                        </div>
                    </div>
                </div>

                <div class="bg-gray-300 rounded-sm">
                    <div class="flex items-center px-4 py-3 border-b
border-gray-400 last:border-b-0">
                        <div class="flex items-center justify-center
mr-2">
                            <button class="text-green-600">
                                <svg class="w-5 h-5" fill="none"
                                     stroke="currentColor" viewBox="0 0 24 24"
                                     xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round"
                                                                              stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            </button>
                        </div>

                        <div class="w-full">
                            <input
                                type="text"
                                placeholder="Digite a sua tarefa"
                                value="Estudar Vue 3"
                                readonly
                                class="line-through bg-gray-300
placeholder-gray-500 text-gray-700 font-light focus:outline-none block
w-full appearance-none leading-normal mr-3"
                            >
                        </div>

                        <div class="ml-auto flex items-center
justify-center">
                            <button class="focus:outline-none">
                                <svg
                                    class="ml-3 h-4 w-4 text-gray-500"
                                    viewBox="0 0 24 24"
                                    fill="none"
                                    stroke="currentColor"
                                    xmlns="http://www.w3.org/2000/svg"
                                >
                                    <path
                                        d="M19 7L18.1327 19.1425C18.0579
20.1891 17.187 21 16.1378 21H7.86224C6.81296 21 5.94208 20.1891 5.86732
19.1425L5 7M10 11V17M14 11V17M15 7V4C15 3.44772 14.5523 3 14 3H10C9.44772
3 9 3.44772 9 4V7M4 7H20"
                                        stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                    />
                                </svg>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            <!--/ Todo items -->

            <!-- Todo empty -->
            <div class="text-center text-lg text-gray-500">
                Você ainda não tem nenhuma tarefa.
            </div>
            <!--/ Todo empty -->
        </div>
    </div>
    <!--/ Content -->
</template>

<script>
export default {
  name: 'App',
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
