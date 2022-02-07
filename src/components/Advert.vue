<template>
  <div class="h-4/6 bg-secondary flex lg:mr-32 relative">
    <div class="bg-primary w-16 sm:w-20 flex flex-col items-center pt-10">
      <div>
        <div
          class="cursor-pointer transition-all"
          @click="sidenote = 1"
          :class="
            sidenote == 1 ? 'text-lg text-gray-700' : 'text-sm text-gray-300'
          "
        >
          01
        </div>
        <div
          class="my-1 rounded-lg mx-auto transition-all"
          style="width: 2px"
          :class="sidenote == 1 ? 'bg-gray-700 h-10' : 'bg-gray-300 h-8'"
        ></div>
        <div
          class="cursor-pointer transition-all"
          @click="sidenote = 2"
          :class="
            sidenote == 2 ? 'text-lg text-gray-700' : 'text-sm text-gray-300'
          "
        >
          02
        </div>
        <div
          class="my-1 rounded-lg mx-auto transition-all"
          style="width: 2px"
          :class="sidenote == 2 ? 'bg-gray-700 h-10' : 'bg-gray-300 h-8'"
        ></div>
        <div
          class="cursor-pointer transition-all"
          @click="sidenote = 3"
          :class="
            sidenote == 3 ? 'text-lg text-gray-700' : 'text-sm text-gray-300'
          "
        >
          03
        </div>
        <div
          class="my-1 rounded-lg mx-auto transition-all"
          style="width: 2px"
          :class="sidenote == 3 ? 'bg-gray-700 h-10' : 'bg-gray-300 h-8'"
        ></div>
      </div>
      <div class="my-1">
        <div class="my-2">
          <img src="../assets/instagram.png" alt="" class="h-6" />
        </div>
        <div class="my-2">
          <img src="../assets/linkedin.png" alt="" class="h-6" />
        </div>
        <div class="my-2">
          <img src="../assets/twitter.png" alt="" class="h-6" />
        </div>
        <div class="my-2">
          <img src="../assets/facebook.png" alt="" class="h-6" />
        </div>
      </div>
    </div>
    <div
      class="bg-secondary flex flex-col flex-1 pl-16 justify-center relative"
    >
      <h1 class="text-gray-700 my-4 text-6xl">Winter 21'</h1>
      <div class="h-2/6 w-5/12">
        <span class="text-gray-500 text-sm text-size"
          >Winter layer season is here. Check out our trendy new winter
          collection to stay warm in style.</span
        >
      </div>
      <div
        class="h-1/4 flex text-gray-400 text-sm font-semibold attributes flex-to-col w-full"
      >
        <div class="h-full w-32 flex-to-row width-bigger">
          <div>
            <span>Price : </span>
          </div>
          <div class="my-2 text-gray-700 font-bold tracking-tight">
            <span>$ 117.99</span>
          </div>
        </div>
        <div class="h-full w-32 flex-to-row width-bigger">
          <span>Color : </span>
          <div class="my-2 flex">
            <div class="relative cursor-pointer" @click="picked = 0">
              <div
                class="rounded-full border-2 border-gray-300 mr-3"
                :class="picked == 0 ? '' : 'invisible'"
                style="padding: 2.5px; height: 18px; width: 18px"
              ></div>
              <div
                class="absolute bg-gray-300 rounded-full top-by-3"
                style="height: 12px; width: 12px"
              ></div>
            </div>
            <div class="relative cursor-pointer" @click="picked = 1">
              <div
                class="rounded-full border-2 border-gray-500 mr-3"
                :class="picked == 1 ? '' : 'invisible'"
                style="padding: 2.5px; height: 18px; width: 18px"
              ></div>
              <div
                class="absolute bg-gray-500 rounded-full top-by-3"
                style="height: 12px; width: 12px"
              ></div>
            </div>
            <div class="relative cursor-pointer" @click="picked = 2">
              <div
                class="rounded-full border-2 border-gray-700 mr-3"
                :class="picked == 2 ? '' : 'invisible'"
                style="padding: 2.5px; height: 18px; width: 18px"
              ></div>
              <div
                class="absolute bg-gray-700 rounded-full top-by-3"
                style="height: 12px; width: 12px"
              ></div>
            </div>
          </div>
        </div>
        <div class="h-full w-32 flex-to-row width-bigger">
          <span>Size : </span>
          <div class="flex my-3">
            <div
              class="mr-3 cursor-pointer"
              @click="size = 0"
              :class="size == 0 ? 'text-gray-700' : ''"
            >
              S
            </div>
            <div
              class="mr-3 cursor-pointer"
              @click="size = 1"
              :class="size == 1 ? 'text-gray-700' : ''"
            >
              M
            </div>
            <div
              class="mr-3 cursor-pointer"
              @click="size = 2"
              :class="size == 2 ? 'text-gray-700' : ''"
            >
              L
            </div>
            <div
              class="cursor-pointer"
              @click="size = 3"
              :class="size == 3 ? 'text-gray-700' : ''"
            >
              XL
            </div>
          </div>
        </div>
      </div>
      <div class="flex items-start shop-attributes">
        <div class="border-focus bg-primary border-2 px-10 py-3 mb-10">
          <span>Shop now</span>
        </div>
        <div class="mt-3">
          <i class="fa fa-heart-o text-xl mx-3" aria-hidden="true"></i>
          <i class="fa fa-shopping-basket text-xl mx-3" aria-hidden="true"></i>
        </div>
      </div>
      <img
        src="../assets/advert.png"
        alt=""
        class="h-full absolute top-0 right-0 lg:-right-12"
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      picked: 0,
      size: 0,
      sidenote: 0,
    };
  },
};
</script>

<style scoped>
.top-by-3 {
  top: 3.2px;
  left:3.2px;
}
@media (max-width: 800px) {
  .attributes {
    padding: 20px 0px;
    position: absolute;
    bottom: -100px;
    left: 0;
  }
  .shop-attributes {
    padding: 20px 0px;
    position: absolute;
    bottom: -200px;
    left: 0;
  }
  .width-bigger {
    width: 30%;
  }
}
.top-by-3 {
  top: 3.3px;
}
@media (max-width: 440px) {
  .shop-attributes {
    padding: 20px 0px;
    position: absolute;
    bottom: -280px;
    left: 0;
  }
  .top-by-3 {
    top: 3px;
  }
  .width-bigger {
    width: 50%;
  }
  .disp-none {
    display: none;
  }
  .flex-to-col {
    flex-direction: column;
    align-items: center;
  }
  .text-size {
    font-size: 10px;
  }
  .flex-to-row {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }
}
</style>
