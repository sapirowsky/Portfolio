<template>
    <div class="bg-darkBg text-slate-50 font-mono h-screen flex">
        
        <div class="relative flex-1 hidden w-0 lg:block">
            <img class="absolute inset-0 object-cover w-full h-full" src="https://images.unsplash.com/photo-1660809359252-da1452fc333a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2072&q=80" alt="do smothing great">
            <nuxt-img 
                loading="lazy"
                preset="blog"
                class="absolute inset-0 object-cover w-full h-full" 
                src="https://images.unsplash.com/photo-1660809359252-da1452fc333a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2072&q=80" 
                alt="do something great"
                width="1920px"
                height="1080px"
                @click="showCarousel(post, 0)" />
        </div>
        <div class="flex flex-col justify-center items-center flex-1 px-4 py-12 sm:px-6 lg:flex-none lg:px-20 xl:px-24">
            
            <div class="absolute flex items-start w-full h-full max-w-sm mx-auto lg:w-96">
                <div class="pt-10 w-full flex flex-col items-end">
                    <span class="flex flex-col text-gray-400">
                        kamilkruszano@gmail.com
                    </span>
                    <span class="flex flex-col font-bold text-xl">
                        {{ creator }}
                    </span>
                </div>
            </div>
            <div class="flex items-center w-full h-full max-w-sm mx-auto lg:w-96">

                <div class="pt-5 w-full flex flex-col items-end">
                    <h1 class="flex flex-col font-bold text-3xl">
                        <span class="flex justify-end">Under</span>
                        <span>Construction</span>
                    </h1>
                    <p>Strona jest w budowie!</p>

                    <ProgressBar class="mt-12" />

                </div>

            </div>

        </div>

    </div>
</template>
<script setup>
    useHead({
    htmlAttrs: {
      lang: 'pl'
    },  
    title: 'Sapyr Portfolio',
    meta: [
    {
        hid: 'description',
        name: 'description',
        content: 'You can find sapyr\'s portfolio here!'
    }
    ],
  })
  const creator = "<KamilKruszona />"
</script>