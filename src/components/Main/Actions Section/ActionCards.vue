<script>
export default {
    name: "ActionsCards",
    data() {
        return {
            textCards: [
                "Academic professional program in social media",
                "President's speech at the annual meeting",
                "International business trip in Shanghai",
                "Technology workshop with education theme",
                "Donation of clothes and food to the partner NGO",
                "Confraternization of procurement team"
            ]
        }
    }

}
</script>

<template>

    <div class="card" v-for="(text, index) in textCards" :info="text" :key="index">

        <!-- Immagine -->
        <img :src="'src/assets/img/project-' + (index + 1) + '.jpg'" :alt="'image project ' + (index + 1)">

        <!-- Testo -->
        <div class="text">
            {{ text }}
        </div>
    </div>


</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;

.card {
    height: 280px;
    width: 280px;
    position: relative;
    border-radius: 10px;
    cursor: pointer;

    &:hover {
        box-shadow: 0px 0px 10px gray
    }

    img {
        width: 100%;
        border-radius: 10px;
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
