<script>
    import AppleStore from './AppleStore.svelte';
    import GooglePlay from './GooglePlay.svelte';
</script>

<ul>
    <li><AppleStore/></li>
    <li><GooglePlay/></li>
</ul>

<style>
    li {
        list-style-type: none;
    }

    ul {
        display: flex;
        gap: 10px;
    }
</style>