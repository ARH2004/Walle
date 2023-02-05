<template>
    <div class="footer">
        <div class="container">
            <div class="footer__items">
                <div class="footer__text">
                    <ul class="footer__list-one" v-for="l in lawArr" :key="l.id">
                        <li>IQMO.RU - Все права защищены</li>
                        <li>{{ l.inn }}</li>
                        <li>{{ l.ip }}</li>
                        <li>{{ l.tel }}</li>
                        <li>{{ l.mail }}</li>
                    </ul>
                </div>
                <div class="footer__card">
                    <div class="footer__mony">
                        <h4 class="footer__price">Принимаем к оплате:</h4>
                        <div class="footer__img">
                            <img class="footer__cards" src="@/assets/images/visa.png" alt="visa">
                            <img class="footer__cards" src="@/assets/images/master-card.png" alt="master-card">
                            <img class="footer__cards" src="@/assets/images/mir.png" alt="mir">
                        </div>
                        <h4 class="footer__block">Платеж защищен</h4>
                        <div class="footer__img-block">
                            <img class="footer__cards" src="@/assets/images/hhtp.png" alt="hhtp">
                            <img class="footer__cards" src="@/assets/images/lock.png" alt="lock">
                            <img class="footer__cards" src="@/assets/images/prw.png" alt="prw">
                            <img class="footer__cards" src="@/assets/images/pci.png" alt="pci">
                        </div>
                    </div>
                </div>
                <div class="footer__polit">
                    <ul class="footer__list-three" v-for="l in lawArr" :key="l.id">
                        <li class="footer__lsch">{{ l.pol }}</li>
                        <li>{{ l.off }}</li>
                        <li>{{ l.rem }}</li>
                        <li>{{ l.polit }}</li>
                        <li>{{ l.mony }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'v-footer',
    data() {
        return {
            lawArr: [
                { id: Date.now(), inn: '032356620546', ip: 'Романюк Андрей Юрьевич', tel: '+7(995) 233 90 09', mail: 'support@iqmo.ru' },
                { id: Date.now(), pol: 'Политика конфиденциальности', off: 'Оферта', rem: 'Отменить подписку', polit: 'Политика обработки данных', mony: 'Тарифы' }
            ]
        }
    }
}
</script>
<style lang="scss">
.container {
    width: 1100px;
    margin: 0 auto;
}

.footer {
    margin-top: 60px;
    padding-bottom: 40px;

    &__items {
        display: flex;
        justify-content: space-between;
    }

    &__img-block {
        padding-top: 15px;
    }

    &__list-one li {
        color: white;
        padding-top: 10px;
    }

    &__lsch {
        margin-top: -10px;
    }

    &__list-three li {
        color: white;
        padding-bottom: 10px;
    }

    &__img {
        display: flex;
        margin-top: 15px;
    }

    &__block {
        padding-top: 15px;
        color: white;
        letter-spacing: 0.01em;
        font-weight: 600;
        font-size: 14px;
        line-height: 150%;
    }

    &__cards {
        padding-right: 30px;
    }

    &__price {
        color: white;
        letter-spacing: 0.01em;
        font-weight: 600;
        font-size: 14px;
        line-height: 150%;
    }

    &__item {}

    &__card {}

    &__polit {}
}
</style>