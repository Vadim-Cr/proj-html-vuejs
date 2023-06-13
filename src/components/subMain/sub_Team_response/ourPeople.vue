
<script>

export default {
    name: "ourPeople",
    // created the array of objects 
    data() {
        return {
            // created the array for the ourPeople

            persons: [
                { image: '/img/column1-image1.jpg', name: 'Deborah Brown' },
                { image: '/img/column1-image2.jpg', name: 'Allen Lucas' },
                { image: '/img/column1-image3.jpg', name: 'Muriel Potter' },
                { image: '/img/column1-image4.jpg', name: 'Ken Douglas' },
                { image: '/img/column1-image5.jpg', name: 'Loretta Harris' },
                { image: '/img/column1-image6.jpg', name: 'Phil Russell' },
            ],

        }
    },

}
</script>


<template>
    <div class="myTeamContainer">
        <h3>Our People</h3>
        <div v-for="(employe, index) in persons" :key="index" class="myTeamPresentation">
            <img :src="employe.image" :alt="employe.name">
            <p>{{ employe.name }}</p>
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

