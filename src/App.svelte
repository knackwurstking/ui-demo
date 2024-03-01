<script>
    import "ui/main.min.css";

    import { UI } from "ui";

    import * as Input from "./lib/components/input";
</script>

<UI.Theme.Root auto />

<main class="is-max ui-container flex column align-center">
    <article>
        <h1>Buttons</h1>
    </article>

    <article>
        <h1>Card</h1>
    </article>

    <article>
        <h1>Dialog</h1>
    </article>

    <article>
        <h1>Drawer</h1>
    </article>

    <article>
        <h1>Flex Grid</h1>
    </article>

    <article class="is-max-width">
        <h1>Input Components</h1>

        <section>
            <Input.Date />
        </section>

        <section>
            <Input.HTMLSelect />
        </section>

        <section>
            <Input.Month />
        </section>

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

    <article>
        <h1>Spinner</h1>
    </article>

    <article>
        <h1>Text Components</h1>
    </article>

    <article>
        <h1>Theme Picker</h1>
    </article>

    <article>
        <h1>(Top) App Bar</h1>
    </article>
</main>

<style>
    :global(html, body, #app) {
        width: 100%;
        height: 100%;
    }
</style>
