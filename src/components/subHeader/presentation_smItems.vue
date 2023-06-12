<script>
import socialIcons from '../socialIcons.vue';

export default {
    name: "presentation_smItems",
    components: {
        socialIcons,
    }
}
</script>

<template>
    <div class="container-up">
        <div class="left">
            <p>Avada & Associates legal team announces deal to open up oil & gas</p>
        </div>

        <div class="right">
            <socialIcons />
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.container-up {
    @include center_between;
    height: 4rem;
    width: 60%;
    background-color: $secondary;

    .left {
        width: 70%;

        p {
            color: $quinary;
        }
    }

    .right {
        width: 30%;
    }
}
</style>
