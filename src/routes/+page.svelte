<script>
    import { base } from '$app/paths';
</script>

<main>
    <h1>Daily Svelte</h1>
    <p>Source <a href="https://github.com/rezbee-dev/svelte-everydays">repository</a></p>

    <section>
        <h2>Challenges:</h2>
        <ul>
            <li><a href="{base}/challenges/counter">Counter</a></li>
        </ul>
    </section>
</main>

<style>
    main {
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        /* justify-content: center; */
        align-items: center;
        margin-top: 12px;
    }

    h2 {
        margin-bottom: 0;
    }

    ul {
        margin-top: 0;
    }
</style>
