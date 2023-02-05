<template>
    <div class="process">
        <div class="container">
            <h2 class="process__title">
                Как проходит курс?
            </h2>
            <div class="process__cards">
                <div class="process__card" v-for="proc in cardsProcess" :key="proc.id">
                    <img class="process__img" :src="require(`../assets/images/${proc.img}`)" alt="img">
                    <h3 class="process__subtitle"> {{ proc.subtitle }}</h3>
                    <p class="process__text">{{ proc.text }}</p>
                </div>
            </div>
            <div>
                <my-button class="process__btn">записаться на курс</my-button>
            </div>
            <div class="process__doctype">
                <div class="process__item" v-for="doc in doctypeArray" :key="doc.id">
                    <img class="process__mini-img" :src="require(`../assets/${doc.img}`)" alt="img">
                    <h4 class="process__sub">{{ doc.sub }}</h4>
                </div>
            </div>
            <div class="process__vector">
                <img src="@/assets/images/vector.png" alt="vector">
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-process',
    data() {
        return {
            cardsProcess: [
                { id: Date.now(), img: 'process1.png', subtitle: 'Лекции', text: 'Получи доступ от преподавателя к записанным видеоматериалам курса' },
                {
                    id: Date.now(), img: 'process2.png', subtitle: 'Платформа', text: 'Обучение происходит на нашей собственной FF-платформе. Благодаря этому, ты можешь проходить курс в удобном для тебя режиме.'
                },
                {
                    id: Date.now(), img: 'process3.png', subtitle: 'Наставник', text: 'Твое обучение будет сопровождаться поддержкой наставника, который будет помогать в прохождении и объяснять то, что тебе непонятно. Все возникшие вопросы по курсу так же можно будет задать наставнику.'
                },
                {
                    id: Date.now(), img: 'process4.png', subtitle: 'Домашние задания', text: 'У нас для тебя есть увлекательнейшие домашние задания, которые помогут тебе закрепить изученный материал и получить фидбэк от наставника.'
                },
            ],
            doctypeArray: [
                { id: Date.now(), img: 'yes.png', sub: 'Доступ ко всем лекциям курса' },
                { id: Date.now(), img: 'yes.png', sub: 'Доступ в IQMO community' },
                { id: Date.now(), img: 'yes.png', sub: 'Индивидуальная проверка домашки' },
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.container {
    width: 1100px;
    margin: 0 auto;
}

.process {
    &__title {
        font-weight: 700;
        font-size: 50px;
        line-height: 62px;
        color: #FFFFFF;
        text-align: center;
    }

    &__vector {
        text-align: center;
        margin-top: 65px;
    }

    &__doctype {
        display: flex;
        justify-content: space-between;
    }

    &__item {
        margin-top: 35px;
        display: flex;
    }

    &__sub {
        color: white;
        font-weight: 400;
        font-size: 18px;
        line-height: 34px;
        padding-top: 10px;
        padding-left: 10px;
    }

    &__cards {
        display: grid;
        gap: 40px;
        grid-template-columns: 1fr 1fr;
        padding-top: 50px;
    }

    &__btn {
        margin-top: 100px;
        width: 1100px;
        height: 177px;
    }

    &__subtitle {
        color: #FFFFFF;
        font-weight: 700;
        font-size: 23px;
        line-height: 22px;
        padding-top: 45px;
    }

    &__text {
        color: #8997AB;
        font-weight: 400;
        font-size: 18px;
        line-height: 34px;
        padding-top: 30px;
    }
}
</style>