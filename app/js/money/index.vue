<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Ada></Ada>
        <Money></Money>
        <Adb></Adb>
        <Finance></Finance>
        <Adc></Adc>
        <Footor cname="mfooter"></Footor>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header.vue";
import Footor from "../public/footer.vue";
import Slider from "./mslider.vue";
import Navbar from "../public/navbar.vue";
import Ada from "./ada.vue";
import Adb from "./adb.vue";
import Adc from "./adc.vue";
import Finance from "./finance.vue";
import Money from "./money.vue";

export default {
    components: {
        Heador,
        Slider,
        Ada,
        Adb,
        Adc,
        Money,
        Finance,
        Footor,
        Navbar
    }
}
</script>

<style lang="scss">
.mfooter{
    margin-right: 0 !important;
    ul{
        li:first-child{
            display: none;
        }
    }
}
</style>
