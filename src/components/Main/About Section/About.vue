<script>
import AboutNumbers from './AboutNumbers.vue'
export default {
    name: "About",
    components: {
        AboutNumbers
    }
}
</script>

<template>
    <div class="left">
        <div class="content">
            <div class="blue-text">
                ABOUT THE NETWORK
            </div>

            <div class="title">
                <div class="bg-title">
                    The
                </div>
                <span>
                    Company
                </span>
            </div>

            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras iaculis diam varius diam
                ultricies lacinia.
            </p>

            <AboutNumbers />

            <div>
                <a href="#" class="button solid">
                    GET IN TOUCH
                </a>

                <a href="#" class="button trasparent">
                    READ MORE
                </a>
            </div>
        </div>

    </div>

    <div class="right"></div>

</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;


.left {
    @include d-flex(center, flex-end);
    flex-direction: column;
    width: 50%;
    height: 100%;
    padding-right: 50px;

    .content {
        width: 55%;

        .blue-text {
            font-size: 10px;
        }

        .title {
            color: $dark-text-color;
            font-weight: bold;
            font-size: 40px;
            margin: 20px 0;
        }

        h3 {
            color: $dark-text-color;
        }

        p {
            color: $text-color;
            font-size: 14px;
        }

        .button {
            margin: 0 10px;
        }

        .button.trasparent {
            color: $primary-color;
            text-align: left;
        }
    }
}

.right {
    width: 50%;
    height: 100%;
    background-image: url("../../../assets/img/about-5.jpg");
    background-size: cover;
    background-position: center;
}
</style>