<script setup>
import { ref } from 'vue';

let likes =ref(0)
let dislikes = ref(0)


function like(){
likes.value++
}
function dislike(){
  dislikes.value++
}

</script>

<template>
  <section class="border-black max-w-[410px] my-0 mx-auto bg-slate-600 ">
    <div class="px-4">
      <div>
        <div class="flex w-[100%] "> 
          <div class=" w-[98%] mt-2"><h1>Historias</h1></div>
          <div class="bg-cyan-700 mt-2 rounded-[5px] p-1"><h3 class="text-white"> Todas </h3></div>
        </div>
        <div class="flex">
          <div class="m-2"> 
          <div class="w-20 h-20 "><img  class=" border-[4px] border-blue-700 rounded-[15px] " src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQs5R95ommverV5hgec4CLkEC3N5k1HNKh9Vw&usqp=CAU" alt=""></div>
          <div class=""><h3 >camila</h3></div>
        </div>
        <div class="m-2"> 
          <div class="w-20 h-20 "><img  class=" border-[4px] border-blue-700 rounded-[15px] " src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQs5R95ommverV5hgec4CLkEC3N5k1HNKh9Vw&usqp=CAU" alt=""></div>
          <div class=""><h3 >camila</h3></div>
        </div>
        <div class="m-2"> 
          <div class="w-20 h-20 "><img  class=" border-[4px] border-gray-700 rounded-[15px] " src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQs5R95ommverV5hgec4CLkEC3N5k1HNKh9Vw&usqp=CAU" alt=""></div>
          <div class=""><h3 >camila</h3></div>
        </div>
        <div class="m-2"> 
          <div class="w-20 h-20 "><img  class=" border-[4px] border-gray-700 rounded-[15px] " src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQs5R95ommverV5hgec4CLkEC3N5k1HNKh9Vw&usqp=CAU" alt=""></div>
          <div class=""><h3 >camila</h3></div>
        </div>
        
        </div>

      </div>

    </div>
    <div class="w-[100%] flex p-4">
      <div class="flex w-[80%]">
        <div> <img class="w-10 h-10 rounded-full" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRA0WLZmT4qwFKnSWz7upAGR0OsKNkx181_lQ&usqp=CAU" alt=""></div>
        <div>
          <h1>mariano perez</h1>
          <h3>hace 10 minutos</h3>
        </div>
      </div>
      <div class="w-[5%]">
        <h3 class="text-red-500">reportar</h3>

      </div>


    </div>
    <div class="px-4 pb-2">
      <img class="rounded-[20px]" src="https://live.staticflickr.com/7328/8717979080_d5ee8a5a77_b.jpg" alt="">
    </div>


    <div class="pt-2 flex px-4">
      <div class="flex">
        <svg   @click="like(likes)" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path class="text-red-600" stroke-linecap="round" stroke-linejoin="round" d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12z" />
        </svg>
        <h3>{{ likes }}</h3>
      </div>



      <div class="flex px-2">
        <svg @click="dislike(dislikes)" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M7.5 15h2.25m8.024-9.75c.011.05.028.1.052.148.591 1.2.924 2.55.924 3.977a8.96 8.96 0 01-.999 4.125m.023-8.25c-.076-.365.183-.75.575-.75h.908c.889 0 1.713.518 1.972 1.368.339 1.11.521 2.287.521 3.507 0 1.553-.295 3.036-.831 4.398C20.613 14.547 19.833 15 19 15h-1.053c-.472 0-.745-.556-.5-.96a8.95 8.95 0 00.303-.54m.023-8.25H16.48a4.5 4.5 0 01-1.423-.23l-3.114-1.04a4.5 4.5 0 00-1.423-.23H6.504c-.618 0-1.217.247-1.605.729A11.95 11.95 0 002.25 12c0 .434.023.863.068 1.285C2.427 14.306 3.346 15 4.372 15h3.126c.618 0 .991.724.725 1.282A7.471 7.471 0 007.5 19.5a2.25 2.25 0 002.25 2.25.75.75 0 00.75-.75v-.633c0-.573.11-1.14.322-1.672.304-.76.93-1.33 1.653-1.715a9.04 9.04 0 002.86-2.4c.498-.634 1.226-1.08 2.032-1.08h.384" />
        </svg>
        <h3>{{ dislikes }}</h3>
      </div>
    </div>


    <div class="bg-slate-500 flex justify-between p-4 m-4 rounded-[20px]">
      <div class="w-[20px] h-[20px] bg-white  rounded-[5px ] p-4 flex  ">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
        </svg>


      </div>



      <div class="w-[20px] h-[20px] bg-white  rounded-[5px ] p-4   ">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
        </svg>


      </div>





      <div class="w-[20px] h-[20px] bg-white  rounded-[5px ] p-4   ">
        

      </div>




    </div>








  </section>
</template>

