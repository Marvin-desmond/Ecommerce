<template>
  <div class="h-16 sm:h-20 flex items-center justify-between lg:mr-32">
    <div class="flex items-center h-full">
      <div class="w-16 sm:w-20 bg-focus flex self-stretch items-center justify-center">
        <img src="../assets/menu.png" class="h-4" alt="" />
      </div>
      <div class="mx-3">
        <span class="font-semibold">EleShoply.</span>
      </div>
    </div>
    <div class="flex">
      <div class="flex disp-none">
        <i class="fa fa-search text-xl mx-3" aria-hidden="true"></i>
        <i class="fa fa-heart-o text-xl mx-3" aria-hidden="true"></i>
        <i class="fa fa-shopping-basket text-xl mx-3" aria-hidden="true"></i>
      </div>
      <div class="bg-focus text-white text-sm px-5 py-1 ml-7">Login</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@media (max-width: 440px) {
  .disp-none{
      display: none;
  }
  
}
</style>
