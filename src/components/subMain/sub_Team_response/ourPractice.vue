
<script>
import teamCard from './teamCard.vue';
import practiceCard from './practiceCard.vue';

export default {
    name: "teamResponse",
    components: {
        teamCard,
        practiceCard
    },
    // created the array of objects 
    data() {
        return {
            // created the array for the NAV
            companySections: [
                {
                    type: 'ourPeople',
                    persons: [
                        { image: '/img/column1-image1.jpg', name: 'Deborah Brown' },
                        { image: '/img/column1-image2.jpg', name: 'Allen Lucas' },
                        { image: '/img/column1-image3.jpg', name: 'Muriel Potter' },
                        { image: '/img/column1-image4.jpg', name: 'Ken Douglas' },
                        { image: '/img/column1-image5.jpg', name: 'Loretta Harris' },
                        { image: '/img/column1-image6.jpg', name: 'Phil Russell' },
                    ],
                },
                {
                    type: 'practiceAreas',
                    areas: [
                        { image: 'imagePath7', area: 'Tax Litigation' },
                        { image: 'imagePath8', area: 'Acquisition' },
                        { image: 'imagePath9', area: 'Financial Advice' },
                        { image: 'imagePath10', area: 'International' },
                        { image: 'imagePath11', area: 'Oil and Gas' },
                        { image: 'imagePath12', area: 'Capital Markets' },
                    ],
                },
                {
                    type: 'publications',
                    publications: [
                        { image: 'imagePath13', title: 'Low Oil Prices' },
                        { image: 'imagePath14', title: 'Cost of Divorce' },
                        { image: 'imagePath15', title: '2015 Tax Laws' },
                        { image: 'imagePath16', title: 'Surveys Matter' },
                        { image: 'imagePath17', title: 'In-house Work' },
                        { image: 'imagePath18', title: 'Obama Care' },
                    ],
                },]
        }
    },

}
</script>


<template>
    <div class="myTeamContainer">
        <h1>GLOBAL CHALLENGE. WORLD CLASS RESPONSE</h1>
        <div class="myTeamPresentation">
            <teamCard :mySections="companySections" />
            <!-- <practiceCard :mySections="companySections" /> -->
            <!-- <publicationCard :mySections="companySections" /> -->
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.myTeamContainer {
    background-color: $tertiary;
    padding-top: 8rem;
    font-family: $familyFont;
    border-top: 1px solid #dad9d9;
    text-align: center;

    h1 {
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

    .myTeamPresentation {
        display: flex;
        text-align: center;
        width: 70%;
        margin: auto;
        min-height: 20rem;
        margin-top: 3rem;


    }
}
</style>

