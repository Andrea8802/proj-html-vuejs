<script>
import CardFeedback from './CardFeedback.vue';

export default {
    name: "Feedback",
    components: {
        CardFeedback
    }

}
</script>

<template>

    <!-- Testo blu -->
    <div class="blue-text">
        CUSTOMERS TESTIMONIALS
    </div>

    <!-- Titolo -->
    <div class="title">
        Trusted

        <!-- Titolo con bg colorato -->
        <div class="bg-title">
            Feedback
        </div>
    </div>

    <!-- Testo -->
    <p>
        We work intensively in search of ideals that can add up in the lives of our customers. This is what moves us and
        we are grateful for the ricognition.
    </p>

    <!-- Lista card -->
    <div class="card-list">
        <CardFeedback />
    </div>
</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;

.title {
    margin: 15px 0;
}

p {
    width: 40%;
    text-align: center;
}

.card-list {
    margin-top: 30px;
    @include d-flex(space-evenly, center);
    gap: 28px;
}
</style>