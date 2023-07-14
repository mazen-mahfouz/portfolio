<template>
  <div class="w-[95%] m-auto flex justify-center items-center flex-col py-[50px]">
    <div class="w-full lg:w-[85%] flex flex-col-reverse  lg:flex-row justify-between items-center gap-x-[80px] gap-y-[30px] py-[30px]">
        <div class="flex flex-col justify-start items-center">
            <div class="w-full lg:w-[min-content] flex flex-col text-center lg:text-left justify-center lg:justify-start items-center lg:items-start">
                <div class="w-full flex text-center lg:text-left justify-center lg:justify-start">
                    <h1 class="typingEffect lg:ml-0 sm:text-4xl text-[7.2vw]  pl-4 font-semibold font-mono text-slate-800 dark:text-slate-200 self-center lg:self-start flex lg:block items-center justify-center flex-col  transition-all overflow-hidden whitespace-nowrap tracking-[0.15em] mx-auto my-0  py-1 animate-[typing_3s_steps(30,end)]">
                        <div class="w-[60vw] sm:w-[293px] transition-all duration-1000 h-[1px] bg-gradient-to-r from-teal-600 to-purple-600 "></div>
                        <p>Hi I'm Mazen</p>
                        <div class="w-[90vw]  sm:w-[440px] transition-all duration-1000 h-[1px] bg-gradient-to-r from-teal-600 to-purple-600 "></div>
                        <p>Frontend Developer</p>
                        <div class="w-[90vw]  sm:w-[440px] transition-all duration-1000 h-[1px] bg-gradient-to-r from-teal-600 to-purple-600 "></div> 
                    </h1>
                </div>
                <p class="w-full dark:text-slate-400 text-[16px] sm:text-[auto] text-slate-700 my-5 px-2">I can design and build your website or web application using a lot of web technologies like vue.Js tailwind scss firebase and more</p>
                <a href="https://api.whatsapp.com/send/?phone=201097266969&text&type=phone_number&app_absent=0" class="flex gap-[10px] items-center  hover:from-cyan-700 hover:to-blue-800 px-3 py-2 bg-gradient-to-r from-cyan-600 to-blue-700  text-white rounded-lg"><p class="whitespace-pre">Contact with me</p> <i class="fa-solid fa-arrow-right  text-white text-[14px] rounded-lg transition-all ease-in duration-700"></i></a>
            </div>
        </div>
        <div>
            <div class=" bg-black/0 w-fit h-fit flex items-center flex-row  relative">
                <div class=" self-center   w-[95%] h-[280px] max-w-[300px] min-w-[280px] overflow-hidden flex justify-center items-center  rounded-[93%_90%_95%_87%]     border-4 dark:border-slate-900 border-whtie  ring-2  bg-gradient-to-t from-[#7309ec]  dark:to-[#454a75]  to-[#1f2669]">
                    <img src="../image/me.png" class="w-[200px]" alt="">
                </div>
                <div class=" w-9 h-9 rounded-lg absolute right-4 backdrop-blur-md  self-start flex items-center justify-center mt-5 animate-bounce ">
                    <img src="../image/vue.png" class="w-[30px]" alt="">
                </div>
                <div class=" w-9 h-9 rounded-lg absolute left-4 backdrop-blur-md  self-start flex items-center justify-center  mt-5 animate-bounce ">
                    <img src="../image/Tailwind.png" class="w-[30px]" alt="">
                </div>
                <div class=" w-9 h-9 rounded-lg absolute bottom-0 right-4 backdrop-blur-md  self-start flex items-center justify-center -mt-5 animate-bounce ">
                    <img src="../image/sass.png" class="w-[30px]" alt="">
                </div>
            </div>
        </div>
    </div>
    <div class="w-[70%] h-[1px] bg-slate-700 mt-20"></div>
  </div>
</template>


<script>

export default {
  name: "HeaderPage",

  data() {
      return {                                                                                                                              
      }
  },
    
};
</script>

<style lang="scss" scoped>
    .typingEffect {
    width: 0;
    overflow: hidden; /* Ensure the text is not visible until the typewriter effect*/
    white-space: nowrap; /* Keeps the text on a single line */
    animation:typing 2s steps(30) forwards;
  }

/* The typing animation */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}
</style>