<template lang="js">
    <div>
        <button :type="type">
            <slot></slot>
        </button>
    </div>
</template>
<script>
export default {
    name: 'ButtonMain',
    props: {
        type: {
            type: String,
            default: 'button'
        }

    }
}
</script>
<style lang="scss">
    width: 349px;
height: 48.56px;
left: 510px;
top: 488px;

background: #FF662D;
</style>