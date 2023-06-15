<script>
import BottomFooter from './subFooter/bottomFooter.vue';
import letsWorkTogether from './subFooter/letsWorkTogether.vue';


export default {
    name: "AppFooter",
    components: {
        letsWorkTogether,
        BottomFooter
    }
}


</script>

<template>
    <div class="containerFooter">
        <letsWorkTogether />
        <BottomFooter />

    </div>
</template>

<style lang="scss" scoped>
@use '../components/style/partials/variables' as *;
@use '../components/style/general.scss' as *;

.containerFooter {
    min-height: 10rem;
    // margin-top: 8rem;
    width: 100%;
    background-color: $secondary;
}
</style>
