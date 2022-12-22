<script>

export default {
    name: "MiddleJumbotron"
}
</script>

<template>
    <div class="middle">
        <div class="text">
            <div class="blue-text">
                HUMAN RESOURCES
            </div>

            <h2>
                Get More Productivity
                <div class="block"></div>
            </h2>

            <p>
                Plannig, recruiment and selection process and performance evaluation of employees
            </p>

            <a href="#" class="button solid">
                GET IN TOUCH
            </a>

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

        .block {
            background-color: $dark-primary-color;
            width: 105%;
            height: 30px;
            position: absolute;
            bottom: 15px;
            left: 2px;
            z-index: -1;
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