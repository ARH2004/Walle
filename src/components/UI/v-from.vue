<template>
    <from>
        <input v-moedl="int" class="input" type="text" placeholder="Ваш email:">
    </from>
</template>
<script>
export default {
    name: 'my-from',
    data() {
        return {
            int: ''
        }
    }
}
</script>
<style lang="scss" scoped>
.input {
    background: #393C57;
    border: 1px solid #E2521D;
    border-radius: 8px;
    width: 458px;
    height: 60px;
    color: white;
    color: white;
    font-weight: 500;
    font-size: 18px;
    line-height: 120%;
    padding: 20px 0 18px 27px;
}

::placeholder {
    color: white;
    font-weight: 500;
    font-size: 18px;
    line-height: 120%;
    padding: 20px 0 18px 27px;
}

:focus::placeholder {
    color: transparent;
}
</style>