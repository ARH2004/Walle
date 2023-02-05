<template>
    <div class="concept">
        <div class="container">
            <div class="concept__item">
                <h1 class="concept__title">КОНЦЕПТ АРТ</h1>
                <p class="concept__text">
                    Научись мыслить, как концепт-художник, придумывать и воплощать в жизнь оригинальные идеи
                </p>
            </div>
            <my-button class="concept__btn">записаться на курс</my-button>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-concept'
}
</script>
<style lang="scss" scoped>
.concept {
    background: url('@/assets/images/orangeRobot.png') no-repeat;
    background-size: cover;
    min-height: 100vh;

    &__title {
        padding-top: 175px;
        font-weight: 700;
        font-size: 70px;
        line-height: 65px;
        color: white;
        max-width: 350px;
    }

    &__text {
        font-weight: 400;
        font-size: 20px;
        line-height: 24px;
        max-width: 430px;
        padding-top: 30px;
        color: #FFFFFF;
    }

    &__btn {
        margin-top: 75px;
        height: 80px;
        width: 370px;
    }
}

.container {
    width: 1100px;
    margin: 0 auto;
}
</style>