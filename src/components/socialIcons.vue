<script>

export default {
    name: "socialIcons",
}
</script>

<template>
    <div class="icons">
        <div class="left">
            <a href="#">

            </a>
        </div>

        <div class="right"></div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.container-up {
    @include center_between;
    height: 10rem;
    width: 60%;
    background-color: $secondary;

    .left {
        p {
            color: $quinary;
        }
    }
}
</style>
