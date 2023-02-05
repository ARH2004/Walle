<template>
    <div class='program'>
        <div class="container">
            <h2 class="program__title">Программа курса</h2>
            <!-- <div class="program__slider"></div> -->
            <my-accardon></my-accardon>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-program'
}
</script>
<style lang="scss">
.container {
    width: 1100px;
    margin: 0 auto;
}

.program {
    margin-top: 115px;

    &__title {
        color: white;
        text-align: center;
        font-weight: 700;
        font-size: 50px;
        line-height: 62px;
    }

    &__clider {
        margin-top: 75px;
    }
}
</style>