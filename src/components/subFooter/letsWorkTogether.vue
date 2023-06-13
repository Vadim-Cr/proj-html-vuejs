<script>

export default {
    name: "letsWorkTogether",
}
</script>
<template>
    <div class="workGrandContainer">
        <div class="workContainer">
            <h1>LET'S WORK TOGETHER</h1>
            <p>
                We work as a single united team with market leading firms around the world and give our clients the highest
                quality advice possible.
            </p>
            <button type="button">
                <a href="#"> MAKE ENQUIRE </a>
            </button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.workGrandContainer {
    padding-top: 7rem;
    background-image: url(../../assets/img/where-we-work-parallax.jpg);
    background-position: bottom;
    background-repeat: no-repeat;
    background-size: cover;
    height: 100%;
    position: relative;
    height: 45rem;
    @include center_flex;

    &::after {
        content: '';
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background-color: $quaternary;
        opacity: 0.1;
    }

    .workContainer {
        width: 40%;
        margin: auto;
        text-align: center;
        height: 60%;
        font-family: $familyFont;
        position: relative;
        z-index: 1;

        h1 {
            color: $tertiary;
            width: 100%;
            position: relative;
            display: inline-block;
            padding-bottom: 1.5em;

            &::after {
                content: "";
                position: absolute;
                left: 40%;
                /* Adjust these values to center the line */
                right: 40%;
                bottom: 0;
                border-bottom: 1px solid #c8c6c6;
                /* Set the border color and width */
            }
        }

        p {
            color: $tertiary;
            font-weight: 600;
            margin-top: 3rem;
            margin-bottom: 3rem;
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

