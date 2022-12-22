<script>

export default {
    name: "RightTopFooter",

}
</script>

<template>

    <div class="right">
        <h3>
            Example inc.
        </h3>

        <div class="text">
            Lorem ipsum dolor sit amet, consectetur adipliscing elit.
        </div>

        <div class="text">
            Praesent diam lacus, dapibus sed imperdiet consectetur.
        </div>

        <div>
            <div class="contact">
                <span class="icon">
                    <fa icon="fa-solid fa-phone" />
                </span>
                +1 (305) 1234-5678
            </div>

            <div class="contact">
                <span class="icon">
                    <fa icon="fa-solid fa-envelope" />
                </span>
                hello@example.com
            </div>

            <div class="contact">
                <span class="icon">
                    <fa icon="fa-solid fa-location-dot" />
                </span>
                Main Avenue, 987
            </div>

            <a href="#" class="button trasparent">
                VIEW MAP
            </a>

        </div>
    </div>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

.right {
    widows: 50%;
    margin-bottom: 100px;

    h3 {
        color: white;
        font-size: 20px;
    }

    .text {
        color: $light-text-color;
        font-size: 14px;
        width: 80%;
        margin: 25px 0;
    }

    .contact {
        color: $primary-color;
        font-size: 15px;
        @include d-flex(flex-start, center);
        gap: 10px;

        .icon {
            background-color: $dark-bg-title;
            @include d-flex(center, center);
            border-radius: 50%;
            width: 40px;
            height: 40px;
            font-size: 18px;
            margin: 8px 0;
        }
    }

    a {
        margin-top: 15px;
        display: inline-block;
    }

}
</style>
