<template>
    <div>
        <h1>{{ message }}</h1>
        <app-input :msg="message" @messageChanged="message = $event"></app-input>
    </div>
</template>
<script>
    import Input from './Input.vue';
    export default {
        data() {
            return {
                message : ' Hello Christopher!',
            }
        },
        components : {
            'app-input' : Input
        }
    }
</script>
