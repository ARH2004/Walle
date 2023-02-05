<template>
    <div class="subs">
        <div class="container">
            <h2 class="subs__title">
                Только сегодня доступ к курсу за <span class="subs__purple">{{ priceSale }} руб</span>*. Вместо <span
                    class="subs__grey">{{ price }}</span> руб.
            </h2>
            <h4 class="subs__warn">
                Заполните форму, чтобы получить доступ к курсу
            </h4>
            <div class="subs__froms">
                <my-from></my-from>
            </div>
            <div class="subs__c">
                <my-button class="subs__btn">Получить доступ</my-button>
            </div>
            <div class="subs__acept">
                <my-acept></my-acept>
                <p class="subs__text-acept">Даю <a class="subs__link"
                        href="https://www.v2b.ru/articles/novoe-soglasie-na-obrabotku-personalnyh-dannyh-2021/#:~:text=%D0%A1%D0%BE%D0%B3%D0%BB%D0%B0%D1%81%D0%B8%D0%B5%20%D0%BD%D0%B0%20%D0%BE%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D1%83%20%D0%BF%D0%B5%D1%80%D1%81%D0%BE%D0%BD%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D1%85%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85,%D0%B4%D0%BB%D1%8F%20%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20%D0%B2%20%D0%BE%D0%BF%D1%80%D0%B5%D0%B4%D0%B5%D0%BB%D0%B5%D0%BD%D0%BD%D1%8B%D1%85%20%D1%86%D0%B5%D0%BB%D1%8F%D1%85."
                        target="_blank" rel="noopener noreferrer">согласие</a> на обработку персональных данных, а также
                    ознакомлен с
                    публичной офертой и тарифами</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-subs',
    data() {
        return {
            priceSale: 29,
            price: 2900
        }
    }
}
</script>
<style lang="scss">
.container {
    width: 1100px;
    margin: 0 auto;
}

.subs {
    margin-top: 25px;
    text-align: center;

    &__title {
        font-weight: 800;
        font-size: 20px;
        line-height: 140%;
        color: white;
    }

    &__froms {
        margin-top: 30px;
    }

    &__acept {
        margin-top: 25px;
        display: flex;
        justify-content: space-between;
        width: 470px;
        position: relative;
        left: 30%;
    }

    &__text-acept {
        color: rgba(255, 255, 255, 0.6);
        ;
        font-weight: 400;
        font-size: 12px;
        line-height: 140%;
    }

    &__link {
        color: white;
        font-size: 14px;
    }

    &__c {
        margin-top: 25px;
    }

    &__btn {
        width: 458px;
        height: 60px;
    }

    &__purple {
        color: #FA4682;
    }

    &__grey {
        color: gray;
    }

    &__warn {
        margin-top: 40px;
        font-weight: 400;
        font-size: 14px;
        line-height: 140%;
        color: white;
    }

    .subs__link:hover {
        color: red;
        transition: 0.3s all;
    }
}
</style>