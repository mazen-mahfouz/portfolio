<template>
  <div class="w-[95%] m-auto flex justify-center items-center flex-col py-[50px]">
    <h1 class="mb-6 text-3xl tracking-tight font-extrabold text-center text-gray-900 dark:text-white ">Contact Us</h1>
    <div class="w-full md:w-[60%] lg:w-[50%]">
      <form action="https://formspree.io/f/mpzevnwv" method="post" class="w-full flex justify-center items-center flex-col gap-[20px]" >
        <div class="w-full relative">
          <label for="name" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Your Name</label>
          <span class="text-[#cecece] absolute top-[5px] right-[10px] text-[10px]" >required</span>
          <input type="text" id="name" name="name" class="shadow-sm bg-gray-50 border-[1px] border-slate-600  dark:border-none outline-none text-gray-900 text-sm rounded-lg  block w-full p-2.5 dark:bg-gray-700 dark:placeholder-gray-400 dark:text-white  dark:shadow-sm-light" placeholder="John doe" required>
        </div>
        <div class="w-full relative">
          <label for="email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Your email</label>
          <span class="text-[#cecece] absolute top-[5px] right-[10px] text-[10px]" >required</span>
          <input type="email" id="email" name ="email"  class="shadow-sm bg-gray-50 border-[1px] border-slate-600  dark:border-none outline-none text-gray-900 text-sm rounded-lg  block w-full p-2.5 dark:bg-gray-700 dark:placeholder-gray-400 dark:text-white  dark:shadow-sm-light" placeholder="name@mail.com" required>
        </div>
        <div class="w-full relative">
          <div class="flex flex-col gap-[8px]">
              <label for="message" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Your message</label>
              <span class="text-[#cecece] absolute top-[5px] right-[10px] text-[10px]">required</span>
              <textarea id="" name="message" placeholder="Your message..." class="min-h-[200px] block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg shadow-sm  border-[1px] border-slate-600  dark:border-none dark:bg-gray-700  dark:placeholder-gray-400 dark:text-white "></textarea>
          </div>
        </div>
        <div class="w-full flex justify-start">
          <div class="w-full lg:w-[170px] relative mt-[10px] flex">
            <input type="submit" value="Send message" class="py-3 flex px-5  text-sm font-medium transition-all text-center bg-gradient-to-tr hover:opacity-95 from-emerald-600 to-emerald-800 hover:from-emerald-500 hover:to-emerald-900 text-white rounded-lg ">
          </div>  
        </div>
      </form>
    </div>
  </div>
</template>


<script>
export default {
  name: "ContactusPage", 
};
</script>

<style lang="scss" scoped>

</style>