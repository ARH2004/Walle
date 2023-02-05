<template>
    <button class="btn">
        <slot></slot>
    </button>
</template>
<script>
export default {
    name: 'my-button'
}
</script>
<style lang="scss" scoped>
.btn {
    background: #E2521D;
    color: white;
    letter-spacing: 3px;
    text-transform: uppercase;
    text-align: center;
    line-height: 34px;
    border-radius: 10px;
}

.btn:hover {
    transition: 0.2s all;
    box-shadow: 0px 0px 55px rgba(202, 0, 80, 0.51);
}
</style>