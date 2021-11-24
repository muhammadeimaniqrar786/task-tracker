<template>
    <button @click="onClick()" :style="{ background: color }" class="btn">{{ title }}</button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        title: {
            type: String,
            default: 'button text',
        },
        color: {
            type: String,
            default: 'Black',
        },
    },
    methods: {
        onClick() {
            console.log('click')
        }
    }
}
</script>
