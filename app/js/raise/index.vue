<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Daily></Daily>
        <In></In>
        <More></More>
        <Footor cname="mfooter"></Footor>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header.vue";
import Footor from "../public/footer.vue";
import Navbar from "../public/navbar.vue";
import Slider from "./rslider.vue";
import Daily from "./daily.vue";
import In from "./in.vue";
import More from "./more.vue";

export default {
    components: {
        Heador,
        Slider,
        Daily,
        In,
        More,
        Footor,
        Navbar
    }
}
</script>

<style lang="scss" module>
.mfooter{
    margin-top: 0 !important;
    ul{
        li:first-child{
            display: none;
        }
    }
}
</style>
