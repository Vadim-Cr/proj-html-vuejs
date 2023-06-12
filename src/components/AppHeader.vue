<script>
import firstHeadContainer from './subHeader/firstHeadContainer.vue';
export default {
    name: "AppHeader",
    components: {
        firstHeadContainer,
    }
}


</script>

<template>
    <div class="container">
        <firstHeadContainer />
    </div>
</template>

<style lang="scss" scoped>
@use '../components/style/partials/variables' as *;
@use '../components/style/general.scss' as *;

.container {
    border-top: 2px solid $primary;
    height: 10rem;
    width: 100%;
    background-color: $secondary;
}
</style>
