<script>
import letsWorkTogether from './subFooter/letsWorkTogether.vue';


export default {
    name: "AppFooter",
    components: {
        letsWorkTogether,
    }
}


</script>

<template>
    <div class="containerMain">
        <letsWorkTogether />

    </div>
</template>

<style lang="scss" scoped>
@use '../components/style/partials/variables' as *;
@use '../components/style/general.scss' as *;

.containerFooter {
    min-height: 10rem;
    margin-top: 28rem;
    width: 100%;
    background-color: $secondary;
}
</style>
