
<script>

export default {
    name: "ourPublications",
    // created the array of objects 
    data() {
        return {
            // created the array for the ourPeople

            publications: [
                { image: '/img/column3-image1.jpg', name: 'Low Oil Prices' },
                { image: '/img/column3-image2.jpg', name: 'Cost of Divorce' },
                { image: '/img/column3-image3.jpg', name: '2015 Tax Laws' },
                { image: '/img/column3-image4.jpg', name: 'Surveys Matter' },
                { image: '/img/column3-image5.jpg', name: 'In-house Work' },
                { image: '/img/column3-image6.jpg', name: 'Obama Care' },
            ],

        }
    },

}
</script>


<template>
    <div class="myTeamContainer">
        <h3>Our Publications</h3>
        <div v-for="(publication, index) in publications" :key="index" class="myTeamPresentation">
            <img :src="publication.image" :alt="publication.name">
            <p>{{ publication.name }}</p>
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

