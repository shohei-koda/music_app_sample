<template>
    <div class="music">
        <at-button @click="showMessage">Show Message</at-button>
    </div>
</template>

<script>

export default {
    methods: {
        pushKey: function() {

        }
    }
}

new Vue({
    props: ['key'],
    methods: {
        showMessage: function() {

        var synth = new Tone.Synth().toMastere();
        synth.triggerAttackRelease('C5', '4n');
            this.$Message('Thanks for using AT-UI')
        }
    }
}).$mount('#app')

</script>

