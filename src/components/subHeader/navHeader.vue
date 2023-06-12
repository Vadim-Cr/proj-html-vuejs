<script>
import navigator from '../navigator.vue';
export default {
    name: "navHeader",
    components: {
        navigator
    }
}
</script>

<template>
    <div class="upContainer">
        <div class="containerNav">
            <div class="leftNav">
                <img src="../../assets/img/avada-law-logo.png" alt="avada_law_logo">
            </div>

            <div class="rightNav">
                <navigator />
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.upContainer {
    width: 100%;
    background-color: $tertiary;
}

.containerNav {
    @include center_between;
    height: 4rem;
    width: 70%;

    .leftNav {
        width: 30%;
    }

    .rightNav {
        width: 70%;
        padding-right: 2.5rem;
    }
}
</style>
