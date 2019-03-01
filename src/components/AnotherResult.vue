<template>
    <div>
        <p>Double Counter: {{ counter }}</p>
        <p>Click Counter: {{ clicks }}</p>
    </div>
</template>

<script>
    import { mapGetters } from 'vuex';

    export default {
        computed: mapGetters({
            counter: 'doubleCounter',
            clicks: 'stringCounter'
        })
    }
</script>
