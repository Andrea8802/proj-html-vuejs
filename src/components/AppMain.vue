<script>
import FeaturesCards from './FeaturesCards.vue';
import About from './About.vue';

export default {
    name: "AppMain",
    components: {
        FeaturesCards,
        About
    }
}
</script>

<template>
    <main>
        <section class="features">
            <FeaturesCards />
        </section>

        <section class="about">
            <About />
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

main {
    .features {
        @include d-flex(center, center);
        height: 480px;
        widows: 100%;
        background-color: $bg-gray;
        gap: 25px
    }

    .about {
        @include d-flex(center, center);
        height: 620px;
        width: 100%;

    }
}
</style>