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
                Get in
                <div class="bg-title">
                    Touch
                </div>
            </div>

            <div class="text">
                We will respond to your message as soon as possible
            </div>

            <form>
                <input type="text" name="name" placeholder="Name" required>

                <input type="email" name="email" placeholder="Email" required>

                <input type="tel" name="phone" placeholder="Phone">

                <select name="type">
                    <option value="">
                        More info
                    </option>
                </select>

                <input type="text" name="message" placeholder="Message" required minlength="10" class="message">

                <button type="submit" class="button solid">
                    SEND
                </button>
            </form>
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

        form {
            margin-top: 30px;
            width: 70%;
            @include d-flex(flex-start, center);
            flex-wrap: wrap;
            gap: 10px;

            input,
            select {
                background-color: #1d1d23;
                color: $light-text-color;
                border: none;
                width: calc(50% - 10px);
                padding: 12px;
                border-radius: 3px;
            }

            select {
                color: $text-color;
            }

            .message {
                width: calc(100% - 10px);
                padding: 10px 10px 100px;
            }

            button {
                border: none;
                margin-top: 15px;
            }
        }



    }
}
</style>
