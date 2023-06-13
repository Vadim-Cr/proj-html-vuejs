<script>

export default {
    name: "askExpert",
}
</script>
<template>
    <div class="envatoGrandContainer">
        <div class="envatoContainer">
            <img src="../../assets/img/envato-logo.png" alt="envato_logo">
            <p>
                "We have worked with Avada Law for the past 15 ears. As we have grown and evolved, what I have valued most
                about our relationship is that Avada lLaw knows us and our business"
            </p>
            <h3>
                <span> Nigel Rawlinson </span>
                <i class="fa-solid fa-circle"></i>
                <span> Senior Partner </span>
            </h3>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.envatoGrandContainer {
    background-image: url(../../assets/img/video_law_home_preview.jpg);
    background-position: bottom;
    background-repeat: no-repeat;
    background-size: cover;
    height: 100%;
    position: relative;
    height: 25rem;
    @include center_between;

    &::after {
        content: '';
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background-color: $quaternary;
        opacity: 0.8;
    }

    .envatoContainer {
        width: 70%;
        margin: auto;
        text-align: center;
        height: 100%;
        font-family: $familyFont;
        position: relative;
        z-index: 1;

        img {
            margin-top: 5rem;
            margin-bottom: 3rem;
        }

        p {
            color: $tertiary;
            font-style: italic;
            margin-bottom: 3rem;
        }

        h3 {
            color: $tertiary;
            position: relative;

            span {
                margin: 1rem;
            }

            i {
                font-size: 0.5rem;
                position: absolute;
                top: 37%;
                right: 48.7%;
            }
        }
    }
}
</style>

