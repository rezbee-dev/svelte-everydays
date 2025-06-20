<script>
    /*
    - Dropdown menu with "one-way flight" & "return flight" options
    - 2 text input fields for start and return dates
    - Button for "book" flight that submits the dates & flight type
    - When "return flight" selected, the "return date" input is enabled, or else its disabled
    - "return date" input must be after the "start" date, or else "book" button will be disabled
    - when date input fields are in invalid format, then book button will be disabled & there will be red error 
    */

   import { base } from "$app/paths";
</script>

<main>
    <section>
        <select name="" aria-labelledby="">
            <option value="oneway">one-way flight</option>
            <option value="twoway">return flight</option>
        </select>
        <input type="date" name="depart">
        <input type="date" name="return">
        <button>Book</button>
    </section>
    <footer>
        <small><a href="{base}/">Home</a></small>
        <small><a href="https://eugenkiss.github.io/7guis/tasks/#flight">Challenge</a></small>
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

    section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
</style>