<template>
    <div :class="baseClass">
        {{ test }}
        <slot />
    </div>
</template>

<script>
export default {
    props: {
        variant: {
            type: String,
            default: ''
        },
        test: {
            type: String,
            default: 'test'
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
}

</script>

<style scoped>
.alert {
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