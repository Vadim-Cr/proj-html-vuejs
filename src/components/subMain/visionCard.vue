<script>

export default {
    name: "card",
    props: {
        visionInfo: Array,
    }
}
</script>

<template>
    <div v-for="(visions, index) in visionInfo" :key="index" class="visionCard">
        <div class="visionIcon">
            <i :class="visions.icon"></i>
        </div>
        <h3>{{ visions.title }}</h3>
        <p>
            {{ visions.text }}
        </p>

    </div>
</template>

<style lang="scss" scoped>
@use '.././style/partials/variables' as *;
@use '.././style/partials/mixins.scss' as *;
@use '.././style/general.scss' as *;


.visionCard {
    width: calc(100% / 4);
    height: 15rem;
    padding: 0.5rem 1.25rem;
    text-align: center;
    font-family: $familyFont;
    background-color: $tertiary;

    .visionIcon {
        font-size: 1.75rem;

        i {
            color: $primary;
        }
    }

    h3 {
        margin: 2rem 0 2rem 0;
    }

    p {
        margin-bottom: 1rem;
        color: $quinary;
    }


}

// border-top: 4px solid $primary;
</style>
