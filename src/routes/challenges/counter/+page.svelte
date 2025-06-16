<script>
    import { base } from "$app/paths"

    let value = $state(0)
    function onclick() {
        value += 1
    }
</script>

<main>
    <section>
        <input type="textfield" {value} readonly/>
        <button {onclick}>Count</button>
    </section>
    <footer>
        <small><a href="{base}/home">Home</a></small>
        <small><a href="https://eugenkiss.github.io/7guis/tasks/">Challenge</a></small>
    </footer>
</main>

<style>
    main {
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    input {
        /* width: 140px; */
        text-align: right;
        padding: 0;
    }

    footer {
        position: absolute;
        bottom: 14px;
    }
</style>