<script>
    import Applications from './Applications.svelte';
</script>

<header>
    <h1>Manifest</h1>
    <h2>Блогером может быть каждый! Участвуйте в рекламных кампаниях и зарабатывайте.</h2>
    <p>Без минимального порога на количество подписчиков.</p>
    <Applications/>
</header>

<style>
    h1, h2, ul, li  {
        margin: 0;
    }

    h1 {
        font-size: 40px;
        margin-bottom: 80px;
    }

    h2 {
        font-size: 60px;
        text-align: center;
        margin-bottom: 30px;
    }

    p {
        font-size: 20px;
        margin-bottom: 60px;
    }

    header {
        background-image: radial-gradient(82.02% 251.79% at 21.05% 76.19%, #3DB6F7 0%, #F2D76F 100%);
        display: flex;
        flex-direction: column;
        padding: 60px 300px calc(100px + 60px) 300px;
        align-items: center;
    }
</style>