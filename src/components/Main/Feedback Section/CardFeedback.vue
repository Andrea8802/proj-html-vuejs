<script>
export default {
    name: "CardFeedback",

}
</script>

<template>
    <div class="card">
        <img src="../../../assets/img/logo-1.png" alt="Logo 1">

        <p>
            Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis auge justo, in accusan orci rhoncus
            at pellentseque.
        </p>

        <div class="text">
            Lorem ipsum dolor sit amet consectetur adipiscing elit.
        </div>

        <div class="icon">
            <fa icon="fa-solid fa-quote-right" />
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;

.card {
    height: 230px;
    width: 300px;
    background-color: white;
    padding: 30px;
    border-radius: 5px;
    color: $text-color;
    font-size: 14px;
    position: relative;

    img {
        width: 40%;
    }

    p {
        margin: 15px 0;
    }

    .icon {
        font-size: 26px;
        color: $light-text-color;
        position: absolute;
        bottom: 28px;
        right: 20px;

    }
}
</style>