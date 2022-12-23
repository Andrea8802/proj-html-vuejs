<script>
export default {
    name: "AboutNumbers",
}
</script>

<template>
    <div class="numbers">
        <div class="card">

            <!-- Numeri casuali azienda (di esempio) -->
            <div class="number">
                {{ Math.floor(Math.random() * (150 - 50 + 1)) + 50 }}
            </div>


            <!-- Titolo -->
            <h3>
                Emplyees
            </h3>

            <!-- Testo -->
            <p>
                Lorem ipsum dolor sit amet.
            </p>
        </div>

        <div class="card">
            <div class="number">

                <!-- Numeri casuali azienda (di esempio) -->
                {{ Math.floor(Math.random() * (100 - 0 + 1)) + 0 }}
            </div>

            <!-- Titolo -->
            <h3>
                Partners
            </h3>

            <!-- Testo -->
            <p>
                Lorem ipsum dolor sit amet.
            </p>
        </div>

        <div class="card">
            <div class="number">

                <!-- Numeri casuali azienda (di esempio) -->
                {{ Math.floor(Math.random() * (200 - 100 + 1)) + 100 }}
            </div>

            <!-- Titolo -->
            <h3>
                Customers
            </h3>

            <!-- Testo -->
            <p>
                Lorem ipsum dolor sit amet.
            </p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../styles/partials/variables' as *;
@use '../../../styles/partials/mixins' as *;


.numbers {
    @include d-flex(center, center);
    flex-direction: row;
    text-align: center;
    margin: 30px 0 50px;

    .card {

        .number {
            color: #01a5a6;
            font-weight: bold;
            font-size: 30px;
            margin-right: 30px;
        }

        h3 {
            font-size: 20px;
            color: $dark-text-color;
            margin: 10px 0;
        }

        p {
            text-align: left;
            padding: 0 20px;
        }
    }
}
</style>