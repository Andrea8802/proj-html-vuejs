<script>

export default {
    name: "TopFooter",
}
</script>

<template>

    <section>
        <div class="left">
            <div class="blue-text">
                SEND A MESSAGE
            </div>

            <div class="title">
                Get in touch
                <div class="bg-title">
                    Touch
                </div>
            </div>

            <div class="text">
                We will respond to your message as soon as possible
            </div>
        </div>

        <div class="right">

        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    background-color: $bg-black;
    height: 1100px;
    width: 100%;
    @include d-flex(center, center);

    .left {
        width: 50%;

        .title {
            font-size: 40px;
            font-weight: bold;
            color: white;
            margin: 20px 0;

            .bg-title {
                background-color: $dark-bg-title;
                color: white;
            }
        }

        .text {
            color: $text-color;
            font-size: 14px;
        }
    }
}
</style>
