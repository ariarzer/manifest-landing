<script>
    export let modificator;
</script>

<ol class={'Slides ' + 'Slides--' + modificator}>
    <slot></slot>
</ol>

<style global>
    .Slides {
        display: flex;
        gap: 30px
    }
</style>