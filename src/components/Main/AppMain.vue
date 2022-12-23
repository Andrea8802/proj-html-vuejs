<script>
import FeaturesCards from './FeaturesCards.vue';
import About from './About Section/About.vue';
import Actions from './Actions Section/Actions.vue';
import Process from './Process.vue';
import Feedback from './Feedback Section/Feedback.vue';

export default {
    name: "AppMain",
    components: {
        FeaturesCards,
        About,
        Actions,
        Process,
        Feedback
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

        <section class="feedback">
            <Feedback />
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

main {
    section {
        @include d-flex(center, center);
        width: 100%;

    }

    .features {
        height: 480px;
        background-color: $bg-gray;
        gap: 25px
    }

    .about {
        height: 620px;
    }

    .actions {
        flex-direction: column;
        background-color: $bg-black;
        height: 1050px;
    }

    .process {
        flex-direction: column;
        height: 580px;
    }

    .feedback {
        height: 580px;
        width: 100%;
        background-color: $bg-gray;
        flex-direction: column;
    }
}
</style>