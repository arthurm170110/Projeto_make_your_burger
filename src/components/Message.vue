<template>
    <div class="message-container" :class="messageType">
        <p>{{ msg }}</p>
    </div>
</template>

<script>
    export default {
        name: 'Message',
        props: {
            msg: String
        }
    }
</script>

<style scoped>
    .message-container.success {
        background-color: #cce5ff;
        color: #004085;
        border: 2px solid #b8daff;
        border-radius: 5px;
        padding: 10px;
        max-width: 400px;
        margin: 30px auto;
    }

    .message-container.error {
        background-color: #ffcccc;
        color: #850000;
        border: 2px solid #ff0000;
        border-radius: 5px;
        padding: 10px;
        max-width: 400px;
        margin: 30px auto;
    }

    .message-container.warning {
        background-color: #ffffcc;
        color: #665500;
        border: 2px solid #ffcc00;
        border-radius: 5px;
        padding: 10px;
        max-width: 400px;
        margin: 30px auto;
    }

</style>