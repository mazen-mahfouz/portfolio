<template>
  <div class="w-[95%] m-auto flex justify-center items-center flex-col py-[50px]">
    <div class="w-[90%] h-[1px] bg-slate-700 mb-20"></div>
    <h1 class="mb-8 text-3xl tracking-tight font-extrabold text-center text-gray-900 dark:text-white ">Projects</h1>
    <div class="w-full">
      <div class="w-full flex flex-wrap justify-center items-stretch gap-[20px]">
        <div v-for="(project, index) in data" :key="index" class="bg-white dark:bg-slate-800 w-[95%] max-w-[280px] dark:shadow-none shadow-[0_0_25px_#726969] rounded-xl">
          <div>
            <img :src="require('../image/' + project.img + '.png')" class="w-full h-full rounded-lg relative ring-1 self-center" alt="">
            <div class="p-2 text-center">
              <p class="opacity-90 text-sm my-2 text-[black] dark:text-[white] mb-[20px]">{{project.description}}</p>
              <div class="flex justify-around items-center p-2  bg-[#0f172a4d] rounded-lg mb-[15px]">
                <img v-for="(skill, index) in project.skills" :key="index" :src="require('../image/' + skill + '.png')" class="w-[25px]" alt="">
              </div>
              <div class="w-full grid grid-cols-[70%_20%] justify-center items-stretch gap-[10px] mb-[10px]">
                <a :href="project.demo">
                  <div class="group py-[5px] bg-pink-500 rounded-xl relative">
                    <h1 class="text-[white] text-[17px] font-medium tracking-wider translate-x-[-10px]">Demo</h1>
                    <i class="fa-solid fa-arrow-right absolute right-[3%] text-pink-500 bg-white px-[10px] group-hover:w-[94%] w-[25%] py-[8px] text-[14px] rounded-lg top-[50%] translate-y-[-50%] transition-all ease-in duration-700"></i>
                  </div>
                </a>
                <a :href="project.code">
                  <div class="py-[5px] bg-pink-500 rounded-lg text-white hover:bg-white hover:text-pink-500 transition-all ease-in duration-700">
                    <i class="fa-solid fa-code "></i>
                  </div>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="w-[90%] h-[1px] bg-slate-700 mt-20"></div>
  </div>
</template>


<script>

import projects from '../assets/projects.json'

export default {
  name: "ProjectPage",
  data() {
    return {
      data: projects
    }
  },
};
</script>

<style lang="scss" scoped>

</style>