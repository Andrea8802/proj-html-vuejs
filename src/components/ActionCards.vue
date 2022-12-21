<script>
export default {
    name: "ActionsCards"

}
</script>

<template>

    <div class="card">
        <img src="../assets/img/project-1.jpg" alt="image project 1">

        <div class="text">
            Academic professional program in social media
        </div>
    </div>

    <div class="card">
        <img src="../assets/img/project-2.jpg" alt="image project 2">

        <div class="text">
            Academic professional program in social media
        </div>
    </div>

    <div class="card">
        <img src="../assets/img/project-3.jpg" alt="image project 3">

        <div class="text">
            Academic professional program in social media
        </div>
    </div>

    <div class="card">
        <img src="../assets/img/project-4.jpg" alt="image project 4">

        <div class="text">
            Academic professional program in social media
        </div>
    </div>

    <div class="card">
        <img src="../assets/img/project-5.jpg" alt="image project 5">

        <div class="text">
            Academic professional program in social media
        </div>
    </div>

    <div class="card">
        <img src="../assets/img/project-6.jpg" alt="image project 6">

        <div class="text">
            Academic professional program in social media
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.card {
    height: 280px;
    width: 280px;
    position: relative;

    img {
        width: 100%;
        border-radius: 10px;
        // filter: brightness(0.6);
        filter: opacity(0.5);
    }

    .text {
        text-align: center;
        color: white;
        font-weight: bold;
        position: absolute;
        bottom: 30px;
        font-size: 20px;
    }
}
</style>
