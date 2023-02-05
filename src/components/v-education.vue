<template>
    <div class="education">
        <div class="container">
            <h2 class="education__title">Чему ты научишься?</h2>
            <div class="education__cards">
                <div class="education__card" v-for="card in cardsArray" :key="card.id">
                    <img alt="shapeNum" :src="require(`../assets/images/${card.img}`)">
                    <p class="education__text">
                        {{ card.text }}
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-education',
    data() {
        return {
            cardsArray: [
                { id: Date.now(), text: 'С нуля создавать стилизованные 3D-модели архитектуры, окружения и персонажей', img: 'shape1.png' },
                { id: Date.now(), text: 'Настраивать базовые материалы создавать простые текстуры', img: 'shape2.png' },
                { id: Date.now(), text: 'Настраивать сцену, освещение и камеру для рендеринга', img: 'shape3.png' },
                { id: Date.now(), text: 'Создавать анимацию разной сложности', img: 'shape4.png' },
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.container {
    width: 930px;
    margin: 0 auto;
}

.education {
    margin-top: 70px;

    &__title {
        color: #FFFFFF;
        text-align: center;
        font-weight: 700;
        font-size: 50px;
        line-height: 62px;
    }

    &__cards {
        margin-top: 30px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    &__card {
        margin-top: 70px;
    }

    &__text {
        margin-top: 30px;
        font-weight: 500;
        font-size: 18px;
        line-height: 34px;
        color: #FFFFFF;
        width: 430px;
    }
}
</style>