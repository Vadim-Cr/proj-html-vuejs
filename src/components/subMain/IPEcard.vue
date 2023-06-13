<script>

export default {
    name: "card",
    props: {
        cardInfo: Array,
    }
}
</script>

<template>
    <div v-for="(info, index) in cardInfo" :key="index" class="IPEcard">
        <img :src="info.image" alt="info.title">
        <h2>{{ info.title }}</h2>
        <p>{{ info.text }}</p>
    </div>
</template>

<style lang="scss" scoped>
@use '.././style/partials/variables' as *;
@use '.././style/partials/mixins.scss' as *;
@use '.././style/general.scss' as *;


.IPEcard {
    width: calc(100% / 3);
    height: 25rem;
    padding: 0.5rem 1.25rem;
    text-align: center;
    font-family: $familyFont;
    background-color: $tertiary;
    border: 1px solid #dad9d9;
    border-top: 4px solid $primary;
    position: relative;

    img {
        height: 15rem;
        object-fit: contain;
    }

    h2 {
        margin: 1rem 0 2rem 0;
        color: $quaternary;
    }

    p {
        margin-bottom: 1rem;
        color: $quinary;
    }


}

// border-top: 4px solid $primary;
</style>
