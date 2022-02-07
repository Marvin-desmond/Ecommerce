<template>
  <div class="flex flex-col flex-1 push-footer lg:mr-20">
    <div class="my-3">
      <span class="text-5xl text-gray-700"> Category </span>
    </div>

    <div class="flex flex-wrap flex-to-col">
      <div
        v-for="(i, index) in icons"
        :key="index"
        class="h-20 text-white flex flex-col items-center justify-center width-bigger cursor-pointer"
        @click="item_picked = index"
        :class="item_picked == index? 'bg-focus':'bg-secondary text-black'"
      >
        <div :class="index == 4 || index == 7 ? 'fab' : 'fa'">
          <i :class="i.icon"></i>
        </div>
        <div>
          <span>{{ i.item }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      item_picked:0,
      icons: [
        {
          item: "Polo shirt",
          icon: "fa-tshirt",
        },
        {
          item: "Socks",
          icon: "fa-socks",
        },
        {
          item: "Shopping bag",
          icon: "fa-shopping-bag",
        },
        { item: "Shoes", icon: "fa-shoe-prints" },
        { item: "Hat", icon: "fa-redhat" },
        { item: "Cart", icon: "fa-shopping-bag" },
        { item: "Socks", icon: "fa-socks" },
        { item: "Redhat", icon: "fa-redhat" },
      ],
    };
  },
};
</script>

<style scoped>
@media (max-width: 800px) {
  .push-footer {
    margin-top: 150px;
  }
}
.width-bigger{
  padding:10px 0;
  width: 12%;
}
@media (max-width: 440px) {
  .push-footer {
    margin-top: 250px;
  }
  .flex-to-col{
    flex-direction: column;
  }
  .width-bigger{
    width:100%;
    justify-content: start;
  }
}
</style>
