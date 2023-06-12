<script>

export default {
    name: "navigator",
    data() {
        return {
            // created the array for the NAV
            navigator: ['Home',
                'Who We Are',
                'What We Do',
                'Where We Work',
                'Careers',
                'Contact',
                'News']
        }
    }
}
</script>

<template>
    <div class="container">
        <ul>
            <!-- * just iterated every item of the NAV -->
            <li v-for="(option, index) in navigator" :key="index">
                <a href="#">{{ option }}</a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use './style/partials/variables' as *;
@use './style/partials/mixins.scss' as *;
@use './style/general.scss' as *;

.container {
    height: 4rem;
    font-family: $familyFont;


    ul {
        @include center_flex;
        justify-content: flex-end;
        list-style: none;
        height: 100%;

        li {
            margin: 0 0.5rem;
            height: 100%;
            display: flex;
            align-items: center;


            a {
                color: $quinary;
                text-decoration: none;
                height: 100%;
                display: flex;
                align-items: center;

                &:hover {
                    border-top: 2px solid $primary;
                    cursor: pointer;
                    color: $primary;

                }
            }
        }
    }
}
</style>
