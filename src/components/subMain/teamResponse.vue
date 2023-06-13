
<script>
import ourPeople from './sub_Team_response/ourPeople.vue';

export default {
    name: "teamResponse",
    components: {
        ourPeople,
    },

}
</script>


<template>
    <div class="myTeamContainer">
        <h1>GLOBAL CHALLENGE. WORLD CLASS RESPONSE</h1>
        <div class="myTeamPresentation">
            <ourPeople />
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

