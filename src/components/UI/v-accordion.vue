<template>
    <div class="accordion" id="accordion">

        <div class="accordion-item" v-for="acc in accordions" :key="acc.id">
            <h3 class="accordion-item-head" v-on:click="accordion">
                {{ acc.title }}
            </h3>
            <div class="accordion-item-body">
                <p class="accordion__text">Примитивы</p>
                <p class="accordion__text">Основы лайна</p>
                <p class="accordion__text">Композиция масс</p>
                <p class="accordion__text">Работа с референсами</p>
            </div>
        </div>

    </div>
</template>
<script>
export default {
    name: 'my-accardon',
    data() {
        return {
            accordions: [
                { id: Date.now(), title: '1. Основы' },
                { id: Date.now(), title: '2. Знакомство в Zbrush' },
                { id: Date.now(), title: '3. Создание персонажа' },
            ],
        }
    },
    methods: {
        accordion(event) {
            const matches = document.querySelectorAll('.accordion-item-head');
            for (let i = 0; i < matches.length; i++) {
                matches[i].classList.remove('active');
            }
            event.target.classList.toggle('active');
        }
    }
}
</script>
<style lang="scss" scoped>
.accordion {
    margin-top: 75px;

    &__text {
        font-weight: 400;
        font-size: 18px;
        line-height: 34px;
        color: #8997AB;
    }
}

.accordion-item {
    position: relative;
    margin-bottom: 20px;
}

.accordion-item-head {
    background: #0E1B28;
    border-radius: 2px;
    height: 100px;
    cursor: pointer;
    color: white;
    font-weight: 600;
    font-size: 15px;
    line-height: 18px;
    padding: 41px 0px 41px 100px;

}


.accordion-item-head:after {
    content: ' > ';
    display: block;
    height: 29px;
    position: absolute;
    right: 25px;
    transform: rotate(90deg) scaleY(2);
    top: 8px;
}

.accordion-item-head.active:after {
    content: ' < ';
}

.accordion-item-head.active {
    background: #E2521D;
    transition: 0.2s ease;
}



.accordion-item-body {
    transition: 1s ease;
    display: none;
    padding: 30px 0px 55px 80px;
}

.accordion-item-head.active+.accordion-item-body {
    display: block !important;
}
</style>