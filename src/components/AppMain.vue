<script>
import FeaturesCards from './Main/FeaturesCards.vue';
import About from './Main/About Section/About.vue';
import Actions from './Main/Actions Section/Actions.vue';
import Process from './Main/Process.vue';

export default {
    name: "AppMain",
    components: {
        FeaturesCards,
        About,
        Actions,
        Process
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

        <section class="actions">
            <Actions />
        </section>

        <section class="process">
            <Process />
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

    .actions {
        @include d-flex(center, center);
        flex-direction: column;
        background-color: $bg-black;
        height: 1100px;
        width: 100%;
    }

    .process {
        @include d-flex(center, center);
        flex-direction: column;
        height: 580px;
        width: 100%;
    }
}
</style>