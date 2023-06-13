<script>

import card from '../subMain/card.vue';
export default {
    name: "companyPresentation",
    data() {
        return {
            // created the array for the NAV
            organizationInfo: [
                {
                    title: 'Who We Are',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Lorem ipsum dolor sit amet consectetur adipisicing elit.Facere inventore, ',


                    buttonText: 'Learn More'
                },
                {
                    title: 'What We Do',
                    text: 'Integer ac risus id nulla pharetra luctus. molestiae, nesciunt aperiam, iste laudantium facilis rerum suscipit sed soluta corporis',
                    buttonText: 'Learn More'
                },
                {
                    title: 'Where We Work',
                    text: 'Cras lobortis tortor ac auctor ornare. quod voluptates.Possimus quam eos, odio sit explicabo dignissimos.',
                    buttonText: 'Learn More'
                }
            ]
        }
    },
    components: {
        card
    }
}
</script>
<template>
    <div class="presentation">
        <card :cardInfo="organizationInfo" />
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.presentation {
    width: 70%;
    @include center_flex;
    height: 25rem;
}
</style>

