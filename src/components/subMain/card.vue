<script>

export default {
    name: "card",
    props: {
        cardInfo: Array,
    }
}
</script>

<template>
    <div v-for="(info, index) in cardInfo" :key="index" class="card">
        <h2>{{ info.title }}</h2>
        <p>{{ info.text }}</p>
        <button type="button">
            <a href="#">
                {{ info.buttonText }}
            </a>
        </button>
    </div>
</template>

<style lang="scss" scoped>
@use '.././style/partials/variables' as *;
@use '.././style/partials/mixins.scss' as *;
@use '.././style/general.scss' as *;


.card {
    width: calc(100% / 3);
    min-height: 20rem;
    padding: 0.5rem 1.25rem;
    text-align: center;
    font-family: $familyFont;
    background-color: $tertiary;
    border: 1px solid #dad9d9;
    border-top: 4px solid $primary;
    position: relative;

    h2 {
        margin: 3rem 0 2rem 0;
    }

    p {
        margin-bottom: 1rem;
        color: $quinary;
    }

    button {
        background-color: $quaternary;
        border: 1px solid $quaternary;
        margin-bottom: 2rem;
        padding: 0.75rem;
        position: absolute;
        bottom: 0%;
        right: 34%;

        &:hover {
            background-color: $primary;
            cursor: pointer;
        }

        a {
            text-decoration: none;
            color: $tertiary;
            font-weight: 600;
        }
    }
}

// border-top: 4px solid $primary;
</style>
