<template>
    <div>
        <p>Double Counter: {{ counter }}</p>
        <p>Click Counter: {{ clicks }}</p>
    </div>
</template>

<script>
    export default {
        computed: {
            counter() {
                return this.$store.getters.doubleCounter;
            },
            clicks() {
                return this.$store.getters.stringCounter;
            }
        }
    }
</script>
