<script>
export default {
    name: "simpleCard",
    props: {
        mySections: Array,
    }
}
</script>

<template>
    <div v-for="(user, index) in " class="simple_Card">
        <img src="" alt="">
        <div class="name">
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '.././style/partials/variables' as *;
@use '.././style/partials/mixins.scss' as *;
@use '.././style/general.scss' as *;

.ourPeople {
    width: calc(100% / 3);

    .teamCard {
        min-height: 15rem;
        padding: 0.5rem 1.25rem;
        text-align: center;
        font-family: $familyFont;

        h3 {
            margin-bottom: 2rem
        }

        .cardElement {
            width: 100%;
            @include center_flex;
            background-color: $secondary;
            padding: 1rem;
            margin-bottom: 1rem;

            .name {
                margin-left: 1rem;

            }
        }


    }

}

// border-top: 4px solid $primary;
</style>
