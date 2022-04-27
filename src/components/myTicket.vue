<template>
  <swiper :scrollbar="{ draggable: true }" class="tickets-list">
    <swiper-slide class="teacher_li">
      <div class="teacher_pW">
        <p class="teacher_p1">111</p>
        <p class="teacher_p2">- 222 -</p>
      </div>
    </swiper-slide>
    <swiper-slide class="teacher_li">
      <div class="teacher_pW">
        <p class="teacher_p1">111</p>
        <p class="teacher_p2">- 222 -</p>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script>
import SwiperCore, {
  Navigation,
  Pagination,
  Scrollbar,
  Autoplay,
} from "swiper";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/scss";
import "swiper/scss/navigation";
import "swiper/scss/pagination";

import {
  ref,
  defineComponent,
  reactive,
  onMounted,
  toRefs,
  nextTick,
} from "vue";

SwiperCore.use([Navigation, Pagination, Scrollbar, Autoplay]);
export default defineComponent({
  name: "index",
  components: {
    Swiper,
    SwiperSlide,
  },
});
</script>

<style lang="scss" scoped>
.tickets-list {
  margin: 0 auto;
  width: 100%;
  height: 100%;
  background-color: #d3d3d3;
  box-shadow: 2.8px 2.8px 2.2px rgba(0, 0, 0, 0.02),
    6.7px 6.7px 5.3px rgba(0, 0, 0, 0.028),
    12.5px 12.5px 10px rgba(0, 0, 0, 0.035),
    22.3px 22.3px 17.9px rgba(0, 0, 0, 0.042);
}
</style>
