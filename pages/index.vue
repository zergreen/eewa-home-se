<template>
  <div class="md:container md:mx-auto">
    <Navbar />

    <Carousel />

    <Baricon />

    <Topmenu />

    <Toprest />

    <Halal />

    <Category />
  </div>
</template>

<script>
import Topmenu from "@/components/homes/Topmenu";
import Toprest from "@/components/homes/Toprest";
import Halal from "@/components/homes/Halal";
import Category from "@/components/homes/Category";

export default {
  components: { Topmenu, Toprest, Halal, Category },
};
</script>
