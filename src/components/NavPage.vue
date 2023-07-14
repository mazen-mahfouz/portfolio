<template>
  <nav class="flex justify-center items-center flex-col">
    <div class=" flex items-center justify-center w-10 h-7 dark:text-white rounded-[4px] my-4 bg-slate-100 cursor-pointer dark:bg-slate-600 dark:hover:bg-sky-900  hover:bg-sky-200 transition-all">
        <button  @click="$store.state.them == 'light'? $store.state.them = 'dark' : $store.state.them = 'light'" class="dark:text-white flex items-center cursor-pointer m-[auto]">
          <i class="fa-regular font-bold text-[18px]" :class="{'fa-moon': $store.state.them == 'light', 'fa-sun': $store.state.them == 'dark'}"></i>
        </button>
    </div>
    <div class="w-[95%] h-[1px] bg-slate-700 m-auto"></div>
  </nav>
</template>


<script>
export default {
  name: "NavBar", 
};
</script>

<style lang="scss" scoped>

</style>