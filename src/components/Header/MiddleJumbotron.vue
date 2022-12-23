<script>

export default {
    name: "MiddleJumbotron"
}
</script>

<template>
    <div class="middle">
        <div class="text">

            <!-- Testo blu -->
            <div class="blue-text">
                HUMAN RESOURCES
            </div>

            <!-- Titolo -->
            <h2>
                Get More Productivity
                <div class="bar"></div>
            </h2>

            <!-- Testo -->
            <p>
                Plannig, recruiment and selection process and performance evaluation of employees
            </p>

            <!-- Bottone solido -->
            <a href="#" class="button solid">
                GET IN TOUCH
            </a>

            <!-- Bottone traparente -->
            <a href="#" class="button trasparent">
                READ MORE
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

.middle {
    height: 80%;

    @include d-flex(flex-start, center);

    h2 {
        color: white;
        font-size: 60px;
        width: 50%;
        position: relative;
        z-index: 10;
        font-weight: 900;
        line-height: 110%;

        .bar {
            background-color: $dark-primary-color;
            width: 95%;
            height: 30px;
            position: absolute;
            bottom: 2px;
            left: 2px;
            z-index: -1;
            border-radius: 3px;
        }
    }

    p {
        color: $light-text-color;
        font-size: 20px;
        width: 60%;
        margin: 20px 0 40px;
    }

    .button {
        margin: 0 10px;
    }
}
</style>