<template>
  <div class="w-[90%] m-auto flex justify-center items-center flex-col py-[50px]">
    <h1 class="mb-6 text-3xl tracking-tight font-extrabold text-center text-gray-900 dark:text-white ">Skills</h1>
    <div class="w-full text-center">
      <div v-for="(skill, index) in skills" :key="index" :class="skill[0,3]" class=" shadow-[5px_0px_40px_-15px] cursor-pointer  w-[120px]  h-28  items-center justify-center hover:scale-110 rounded-3xl hover:shadow-2xl transition-all inline-block m-3">
        <div class=" h-full w-full rounded-3xl bg-gradient-to-r  p-[1px]" :class="skill[0,2]">
            <div class="flex h-full flex-col rounded-3xl w-full items-center justify-center bg-slate-50 dark:bg-gray-900 shadow-xl back">
              <h1 class="text-slate-800 dark:text-[white] text-[16px]">{{skill[0,0]}}</h1>
            <img  width="50" height="50" :src="skill[0,1]" alt="html-5--v1"/>
            </div>
        </div>
      </div>
      <div class="w-[50%] block h-[1px] bg-slate-700 m-auto my-[20px]"></div>
      <div v-for="(skill, index) in skills_tools" :key="index"  :class="skill[0,3]" class="shadow-[5px_0px_40px_-15px] cursor-pointer  w-[120px]  h-28  items-center justify-center hover:scale-110 rounded-3xl hover:shadow-2xl transition-all inline-block m-3">
        <div class=" h-full w-full rounded-3xl bg-gradient-to-r  p-[1px]" :class="skill[0,2]">
            <div class="flex h-full flex-col rounded-3xl w-full items-center justify-center bg-slate-50 dark:bg-gray-900 shadow-xl back">
              <h1 class="text-slate-800 dark:text-[white] text-[16px]">{{skill[0,0]}}</h1>
            <img  width="50" height="50" :src="skill[0,1]" alt="html-5--v1"/>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>

  import html from '../image/html.png'
  import css from '../image/css.png'
  import js from '../image/js.png'
  import vue from '../image/vue.png'
  import nuxt from '../image/nuxt.png'
  import vuex from '../image/vuex.png'
  import sass from '../image/sass.png'
  import tailwind from '../image/Tailwind.png'
  import bootstrap from '../image/bootstrap.png'
  import canvas from '../image/canvas.png'
  import chatgpt from '../image/chatgpt.png'
  import ai from '../image/ai.png'
  import axios from '../image/axios.png'
  import github from '../image/github.png'
  import git from '../image/git.png'
  import keyboard from '../image/keyboard.png'
  import api from '../image/api.png'
  import photoshop from '../image/photoshop.png'

export default {

  name: "SkillsPage", 
  data() {
    return {
      skills: [
        ['Html5', html, 'from-yellow-500 via-orange-600 to-yellow-500', 'shadow-[#ff6d00]'],
        ['Css3', css, 'from-[#039be5] via-[#008de1] to-[#039be5]', 'shadow-[#039be5]'],
        ['Javascript', js, 'from-[#b49a0c] to-[#b49a0c] via-yellow-400', 'shadow-[#b49a0c]'],
        ['Vue', vue, 'from-[#7fc482] via-[#81c784] to-[#7fc482]', 'shadow-[#7fc482]'],
        ['Nuxt', nuxt, 'from-[#7fc482] via-[#81c784] to-[#7fc482]', 'shadow-[#7fc482]'],
        ['Vuex', vuex, 'from-[#4fc08d] via-[#3f7d72] to-[#4fc08d]', 'shadow-[#4fc08d]'],
        ['Scss', sass, 'from-[#e75f8d] via-[#91366e] to-[#e75f8d]', 'shadow-[#e75f8d]'],
        ['Tailwind', tailwind, 'from-[#00acc1]  via-[#00acc1] to-[#00acc1]', 'shadow-[#00acc1]'],
        ['Bootstrap', bootstrap, 'from-purple-400  via-indigo-500 to-purple-400', 'shadow-purple-400'],
        ['Canvas', canvas, 'from-[#4557fb] via-[#b49ee4] to-[#7343fa]', 'shadow-[#7343fa]'],
        ['Axios', axios, 'from-[#029ae1] via-[#029ae1] to-[#83a4bd]', 'shadow-[#83a4bd]'],
        ['Chatgpt', chatgpt, 'from-[#263a64] via-[#51648f] to-[#51648f]', 'shadow-[#51648f]'],
        ['Ai tools', ai, 'from-[#1e88e5]  via-[#feed59] to-[#1e88e5]', 'shadow-[#1e88e5]'],
      ],
      skills_tools: [
        ['Github', github, 'from-[#444444] via-slate-500 to-[#444444]', 'shadow-[#444444]'],
        ['Git', git, 'from-[#f4511e] via-[#793122] to-[#f4511e]', 'shadow-[#f4511e]'],
        ['Rapid Typing', keyboard, 'from-slate-400  via-slate-600 to-slate-400', 'shadow-[#444444]'],
        ['Apis', api, 'from-slate-400  via-slate-600 to-slate-400', 'shadow-[#444444]'],
        ['photoshop', photoshop, 'from-blue-500  via-blue-700 to-blue-500', 'shadow-[#1e88e5]'],

      ]
    }
  },
};
</script>

<style lang="scss" scoped>

</style>