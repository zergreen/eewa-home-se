<template>
  <div class="flex mt-10">
    <span class="mt-4 ml-2">หมวดหมู่อาหาร</span>
    <button
      class="bg-red-800 m-2 hover:bg-red-900 text-white py-1 px-3 rounded"
    >
      ดูเพิ่มเติม
    </button>
  </div>
  <div class="rounded mt-5">
    <div class="container mx-auto">
      <div class="grid grid-cols-3 gap-6">
        <div class="rounded grid place-items-center">
          <img
            class="h-60 rounded object-center"
            src="@/assets\images\013.jpg"
            alt="Sunset in the mountains"
          />
          <div class="mt-3 w-full">
            <p class="text-center text-lg text-gray-700">อาหารตามสั่ง</p>
          </div>
        </div>

        <div class="rounded grid place-items-center">
          <img
            class="h-60 rounded object-center"
            src="@/assets\images\003.jpg"
            alt="Sunset in the mountains"
          />
          <div class="mt-3 w-full">
            <p class="text-center text-lg text-gray-700">ของหวาน</p>
          </div>
        </div>

        <div class="rounded grid place-items-center">
          <img
            class="h-60 rounded object-center"
            src="@/assets\images\004.jpg"
            alt="Sunset in the mountains"
          />
          <div class="mt-3 w-full">
            <p class="text-center text-lg text-gray-700">
              เครื่องดื่ม / น้ำดื่ม
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Category",
};
</script>

<style></style>
