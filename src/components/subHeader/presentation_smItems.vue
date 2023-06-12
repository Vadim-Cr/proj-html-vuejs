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
    width: 70%;
    background-color: $secondary;
    font-family: $familyFont;

    .left {
        width: 80%;

        p {
            color: $quinary;
        }
    }

    .right {
        width: 20%;
        display: flex;
        justify-content: end;
    }
}
</style>
