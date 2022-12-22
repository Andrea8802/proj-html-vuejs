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
    <div class="blue-text">
        CUSTOMERS TESTIMONIALS
    </div>

    <div class="title">
        Trusted
        <div class="bg-title">
            Feedback
        </div>
    </div>

    <p>
        We work intensively in search of ideals that can add up in the lives of our customers. This is what moves us and
        we are grateful for the ricognition.
    </p>

    <div class="card-list">
        <CardFeedback />
        <CardFeedback />
        <CardFeedback />
    </div>
</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;

.title {
    font-size: 40px;
    font-weight: bold;
    color: $dark-text-color;
    margin: 15px 0;
}

p {
    color: $text-color;
    font-size: 14px;
    width: 40%;
    text-align: center;
}

.card-list {
    margin-top: 30px;
    @include d-flex(space-evenly, center);
    gap: 28px;
}
</style>