<script>

export default {
    name: "socialIcons",
    data() {
        return {
            socialMedia: ['fa-brands fa-facebook-f',
                'fa-brands fa-twitter',
                'fa-brands fa-instagram',
                'fa-brands fa-youtube']
        }
    }
}
</script>

<template>
    <div class="icons">
        <a v-for="(icon, index) in socialMedia" :key="index" href="#">
            <i :class="icon"></i>
        </a>
    </div>
</template>

<style lang="scss" scoped>
@use './style/partials/variables' as *;
@use './style/partials/mixins.scss' as *;
@use './style/general.scss' as *;

.icons {
    @include center_between;
    width: 12rem;

    a {

        i {
            font-size: 1.2rem;
            background-color: $primary;
            padding: 0.5rem;
            color: $tertiary;
            border-radius: 8px;
            margin: 0 0.1rem 0 0.1rem;
        }
    }

}
</style>
