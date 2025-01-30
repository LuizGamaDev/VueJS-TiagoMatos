<template>
    <div :class="baseClass">
        <slot />

        <button @click="onClick()">
            x
        </button>
    </div>
</template>

<script>
export default {
    props: {
        variant: {
            type: String,
            default: ''
        },
    },

    computed: {
        baseClass() {
            return [
                'alert',
                this.variant ? `alert-${this.variant}` : ''
            ]
        },
    },

    methods: {
        onClick() {
            this.$emit('close')
            console.log('cliclou!')
        }
    }
}

</script>

<style scoped>
.alert {
    display: flex;
    justify-content: space-between;
    padding: 5px;
    border-radius: 6px;
    color: white;
    text-align: center;
    background-color: #5d5b5b;
}
.alert-success {
    background-color: green;
}
.alert-danger {
    background-color: red;
}
</style>