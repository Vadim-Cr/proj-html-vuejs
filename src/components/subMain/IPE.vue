<script>

import IPEcard from '../subMain/IPEcard.vue';
export default {
    name: "IPE",
    data() {
        return {
            // created the array for the NAV
            details: [
                {
                    image: '/img/law_7.jpg',
                    title: 'International',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                },
                {
                    image: '/img/law_8.jpg',
                    title: 'Partnerships',
                    text: 'Integer ac risus id nulla pharetra luctus.'
                },
                {
                    image: '/img/law_3.jpg',
                    title: 'Excellence',
                    text: 'Cras lobortis tortor ac auctor ornare.'
                }
            ],
        }
    },
    components: {
        IPEcard
    }
}
</script>
<template>
    <div class="IPEBigContainer">
        <div class="IPEContainer">
            <IPEcard :cardInfo="details" />
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.IPEBigContainer {
    color: $secondary;
    height: 35rem;
    @include center_flex;

    .IPEContainer {
        @include center_flex;
        width: 70%;
        margin: auto;
        height: 25rem;
        background-color: $tertiary;
    }
}
</style>

