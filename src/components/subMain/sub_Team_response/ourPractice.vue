
<script>

export default {
    name: "ourPractice",
    // created the array of objects 
    data() {
        return {
            // created the array for the ourPeople

            practices: [
                { image: '/img/column2-image1.jpg', name: 'Tax Litigation' },
                { image: '/img/column2-image2.jpg', name: 'Acquisition' },
                { image: '/img/column2-image3.jpg', name: 'Financial Advice' },
                { image: '/img/column2-image4.jpg', name: 'International' },
                { image: '/img/column2-image5.jpg', name: 'Oil and Gas' },
                { image: '/img/column2-image6.jpg', name: 'Capital Markets' },
            ],

        }
    },

}
</script>


<template>
    <div class="myTeamContainer">
        <h3>Our Practice</h3>
        <div v-for="(practice, index) in practices" :key="index" class="myTeamPresentation">
            <img :src="practice.image" :alt="practice.name">
            <p>{{ practice.name }}</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../style/partials/variables' as *;
@use '../../style/partials/mixins.scss' as *;
@use '../../style/general.scss' as *;

.myTeamContainer {
    width: calc(100% / 3);

    h3 {
        margin-bottom: 3rem;
    }

    .myTeamPresentation {
        @include center_start;
        padding: 1rem;
        background-color: $secondary;
        margin-bottom: 1rem;
        margin-right: 1rem;

        p {
            margin-left: 1.8rem;
            font-weight: bold;
            color: $quinary;
        }
    }
}
</style>

