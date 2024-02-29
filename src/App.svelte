<script>
    import "ui/main.min.css";

    import { UI } from "ui";

    import * as Input from "./lib/components/input";
</script>

<UI.Theme.Root auto />

<main class="is-max ui-container flex column align-center">
    <article class="is-max-width">
        <h1>Input Elements</h1>

        <section>
            <Input.Number />
        </section>

        <section>
            <Input.Search />
        </section>

        <section>
            <Input.Select />
        </section>

        <section>
            <Input.Slider />
        </section>

        <section>
            <Input.Text />
        </section>
    </article>
</main>

<style>
    :global(html, body, #app) {
        width: 100%;
        height: 100%;
    }
</style>
