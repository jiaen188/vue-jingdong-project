<template>
    <section :class="cname">
        <swiper :options="options" :not-next-tick="options.noNextTick">
            <swiper-slide v-for="item in items" :key="item.href">
                <router-link to="{ name: item.href}">
                    <img :src="item.src">
                </router-link>
            </swiper-slide>
            <div class="swiper-pagination" v-if="options.pagination"></div>
        </swiper>
    </section>
</template>

<script>
import { swiper, swiperSlide } from "vue-awesome-swiper";

export default {
    props: {
        options: {
            type: Object,
            default() {
                return {
                    autoplay: true,
                    loop: true,
                    // 是否需要小圆点
                    pagination: {
                        el: ".swiper-pagination"
                    },
                    noNextTick: false
                }
            }
        },
        items: {
            type: Array,
            default() {
                return [{
                  href: "", // 点击图片要跳转的链接
                  src: ""  // 图片的链接
                }]
            }
        }
    },
    components: {
        swiper,
        swiperSlide
    }
}
</script>

<style lang="scss">
@import "~swiper/dist/css/swiper.css"
</style>
