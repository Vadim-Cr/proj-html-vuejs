<script>
export default {
    name: "teamCard",
    props: {
        mySections: Array,
    }
}
</script>

<template>
    <div v-for="(section, index) in mySections" :key="index" class="practiceAreas">
        <div v-if="section.type === 'practiceAreas'" class="practiceCard">
            <h3>Our Practice</h3>
            <div v-for="(person, idx) in section.persons" :key="idx" class="cardElement">
                <img :src="person.image" :alt="person.name">
                <div class="name">
                    {{ person.name }}
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '.././style/partials/variables' as *;
@use '.././style/partials/mixins.scss' as *;
@use '.././style/general.scss' as *;


.practiceAreas {
    width: calc(100% / 3);

    .practiceCard {
        min-height: 15rem;
        padding: 0.5rem 1.25rem;
        text-align: center;
        font-family: $familyFont;

        h3 {
            margin-bottom: 2rem
        }

        .cardElement {
            @include center_flex;
            background-color: $secondary;
            padding: 1rem;
            margin-bottom: 1rem;

            .name {
                margin-left: 1rem;
            }
        }


    }
}

// border-top: 4px solid $primary;
</style>
