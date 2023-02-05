<template>
    <div class="course">
        <div class="container">
            <h2 class="course__title">
                Для кого этот курс?
            </h2>
            <div class="course__wrapper">
                <div class="course__item">
                    <p class="course__orange">Курс подойдет абсолютно любому. Никакими дополнительными знаниями или
                        навыками
                        моделирования обладать не нужно.</p>
                    <p class="course__white">А так же а также курс будет полезен для тех, кто хочет восполнить пробелы в
                        знании программы или получить дополнительные навыки в работе с софтом.
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-course',
}
</script>
<style lang="scss" scoped>
.container {
    width: 1100px;
    margin: 0 auto;
}

.course {
    margin-top: 110px;
    background: url('@/assets/images/orangeRobotLeft.png') no-repeat;
    background-size: cover;
    height: 100vh;

    &__item {
        margin-left: 645px;
    }

    &__orange {
        padding-top: 165px;
        color: #E2521D;
        font-weight: 400;
        font-size: 30px;
        line-height: 52px;
    }

    &__white {
        padding-top: 50px;
        color: #8997AB;
        font-weight: 400;
        font-size: 18px;
        line-height: 34px;
    }

    &__title {
        color: white;
        font-weight: 700;
        font-size: 50px;
        line-height: 62px;
        text-align: center;
    }
}
</style>