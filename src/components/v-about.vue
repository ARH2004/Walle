<template>
    <div class="about">
        <div class="container">
            <div class="about__wrapper wrapper">
                <div class="about__img">
                    <img src="@/assets/images/whiteRobot.png" alt="">
                </div>
                <div class="about__item">
                    <h1 class="about__title">О чем курс?</h1>
                    <h4 class="about__subtitle">На курсе по концепт-арту вы научитесь создавать различные изображения -
                        предметы, персонажей и окружения.</h4>
                    <p class="about__text">
                        Разработка концепта научит вас реализовывать собственные задумки, выстраивать алгоритм для
                        достижения поставленной цели и ориентироваться на результат
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-about'
}
</script>
<style lang="scss">
.container {
    width: 1100px;
    margin: 0 auto;
}

.wrapper {
    display: grid;
    grid-template-columns: 1.3fr 1fr;
}

.about {
    &__title {
        color: white;
        font-weight: 700;
        font-size: 50px;
        line-height: 62px;
    }

    &__subtitle {
        color: #E2521D;
        font-weight: 400;
        font-size: 25px;
        line-height: 40px;
        padding-top: 80px;
    }

    &__text {
        color: #8997AB;
        font-weight: 400;
        font-size: 18px;
        line-height: 34px;
        padding-top: 20px;
    }
}
</style>