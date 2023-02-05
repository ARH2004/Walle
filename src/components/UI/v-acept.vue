<template>
    <div class="acept">
        <form accept-charset="UTF-8">
            <input class="acept__chek" type="checkbox" name="sometext">
        </form>
    </div>
</template>
<script>
export default {
    name: 'my-acept'
}
</script>
<style lang="scss" scoped>
.acept {
    &__chek {
        width: 21px;
        height: 21px;
    }
}
</style>