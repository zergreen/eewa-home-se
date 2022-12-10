<template>
  <div class="flex mt-10">
    <span class="mt-4 ml-2">รวมร้านอาหารที่มีเครื่องหมายฮาลาล</span>
    <button
      class="bg-red-800 m-2 hover:bg-red-900 text-white py-1 px-3 rounded"
    >
      ดูเพิ่มเติม
    </button>
  </div>
  <div class="bg-slate-100 rounded mt-5">
    <div
      class="grid grid-flow-col auto-cols-max overflow-x-auto pt-5 pl-5 pr-5 pb-10"
    >
       <div
        v-for="(model, index) in models"
        :key="index"
        class="w-96 rounded overflow-hidden shadow-lg mr-5"
      >
        <Card
          :ratings="model.ratings"
          :star="model.star"
          :name="model.name"
          :src="model.src"
          :path="model.path"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Halal",
  data() {
    return {
      models: [
        {
          ratings: "10",
          name: "steack",
          star: "3.5",
          src: "https://www.เที่ยวราชบุรี.com/wp-content/uploads/2020/06/sapburi-600-315.jpg",
          path: "/",
        },
        {
          ratings: "10",
          name: "barbecue",
          star: "3.5",
          src: "https://www.เที่ยวราชบุรี.com/wp-content/uploads/2020/06/sapburi-600-315.jpg",
          path: "/test",
        },
        {
          ratings: "10",
          name: "omlet",
          star: "3.5",
          src: "https://www.เที่ยวราชบุรี.com/wp-content/uploads/2020/06/sapburi-600-315.jpg",
          path: "/omlet",
        },
        {
          ratings: "10",
          name: "pizza",
          star: "3.5",
          src: "https://www.เที่ยวราชบุรี.com/wp-content/uploads/2020/06/sapburi-600-315.jpg",
          path: "/pizza",
        },
      ],
    };
  },
};
</script>

<style></style>
