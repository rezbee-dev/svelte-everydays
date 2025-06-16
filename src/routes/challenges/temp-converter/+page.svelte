<script>
    import { base } from "$app/paths"
    let celVal = $state(0)
    let fahrVal = $state(0)

    function toFahr() {
        fahrVal = Number.parseFloat(((celVal * 9/5) + 32).toFixed(2))
    }

    function toCel(){
        celVal = Number.parseFloat(((fahrVal-32) * (5/9)).toFixed(2))
    }
</script>

<main>
    <section>
        <input type="number" name="celsius" bind:value={celVal} oninput={toFahr}>
        <label for="celsius">Celsius = </label>
        <input type="number" name="fahr" bind:value={fahrVal} oninput={toCel}>
        <label for="fahr">Fahrenheit</label>
    </section>
    <footer>
        <small><a href="{base}/">Home</a></small>
        <small><a href="https://eugenkiss.github.io/7guis/tasks/#temp">Challenge</a></small>
    </footer>
</main>

<style>
    main {
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 12px;
    }

    section {
        border: 1px solid black;
        padding: 12px;
    }

    input {
        max-width: 20ch;
    }

    footer {
        position: absolute;
        bottom: 14px;
    }
</style>