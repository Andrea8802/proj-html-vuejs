<script>
export default {
    name: "LeftTopFooter",
}
</script>

<template>
    <div class="left">

        <!-- Testo blu -->
        <div class="blue-text">
            SEND A MESSAGE
        </div>


        <!-- Titolo -->
        <div class="title">
            Get in

            <!-- Titolo con bg colorato -->
            <div class="bg-title">
                Touch
            </div>
        </div>

        <!-- Testo -->
        <div class="text">
            We will respond to your message as soon as possible
        </div>

        <!-- Form -->
        <form>

            <!-- Nome -->
            <input type="text" name="name" placeholder="Name" required>

            <!-- Email -->
            <input type="email" name="email" placeholder="Email" required>

            <!-- N. Telefono -->
            <input type="tel" name="phone" placeholder="Phone">

            <!-- Lista -->
            <select name="type">

                <option value="moreInfo">
                    More info
                </option>

                <option value="preventive">
                    Preventive
                </option>

                <option value="privacy">
                    Privacy Policy
                </option>

                <option value="other">
                    Other
                </option>
            </select>

            <!-- Messaggio -->
            <input type="text" name="message" placeholder="Message" required minlength="10" maxlength="100"
                class="message">

            <!-- Tasto per mandare dati -->
            <button type="submit" class="button solid">
                SEND
            </button>
        </form>
    </div>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

.left {
    width: 50%;

    .title {
        color: white;
        margin: 20px 0;

        .bg-title {
            background-color: $dark-bg-title;
            color: white;
        }
    }

    form {
        margin-top: 30px;
        width: 100%;
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

            &:hover {
                border: 1px solid gray;
            }

            &:not(:hover) {
                border: 1px solid #1d1d23;

            }

            &:focus {
                outline: none;
                border: 1px solid gray;

            }
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
</style>
