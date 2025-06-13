<script>
    let value = $state(0)
    function onclick() {
        value += 1
    }
</script>

<main>
    <section>
        <input type="number" {value} readonly/>
        <button {onclick}>Count</button>
    </section>
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
</style>