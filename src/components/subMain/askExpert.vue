<script>

export default {
    name: "askExpert",
}
</script>
<template>
    <div class="expertGrandContainer">
        <div class="expertContainer">
            <h1>
                QUESTIONS ABOUT JUDICIAL ISSUES? ASK OUR EXPERTS.
            </h1>
            <button type="button">
                <a href="#"> ASK AN EXPERT </a>

            </button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.expertGrandContainer {
    background-color: $primary;
    height: 10rem;
    @include center_between;


    .expertContainer {
        width: 70%;
        @include center_between;
        height: 5rem;
        font-family: $familyFont;

        h1 {
            color: $tertiary;
        }

        button {
            border: 1px solid #3f8982;
            background-color: #3f8982;
            padding: 0.5rem;
            margin-right: 3rem;

            a {
                text-decoration: none;
                color: $tertiary;
                font-weight: bolder;
                font-size: 1rem;
                font-family: $familyFont;


            }

            &:hover {
                background-color: $quaternary;
                cursor: pointer;
            }
        }
    }
}
</style>

