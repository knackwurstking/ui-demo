<script>
    import { UI } from "ui";

    import * as Input from "./lib/components/input";
    import Spinner from "./lib/components/Spinner.svelte";
    import * as Text from "./lib/components/text";
</script>

<UI.Theme.Root auto />

<main class="is-max ui-container flex column align-center">
    <article class="is-max-width">
        <h1>Buttons</h1>

        <section>
            <!-- TODO: ... -->
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Card</h1>

        <section>
            <!-- TODO: ... -->
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Dialog</h1>

        <section>
            <!-- TODO: ... -->
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Drawer</h1>

        <section>
            <!-- TODO: ... -->
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Flex Grid</h1>

        <section>
            <!-- TODO: ... -->
        </section>

        <hr />
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

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Spinner</h1>

        <section
            class="flex align-center justify-center"
            style="position: relative; height: 5em; overflow: hidden;"
        >
            <Spinner />
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Text Components</h1>

        <section>
            <Text.Label />
        </section>

        <section>
            <Text.Primary />
        </section>

        <section>
            <Text.Secondary />
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Theme Picker</h1>

        <section>
            <!-- TODO: ... -->
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>(Top) App Bar</h1>

        <section>
            <!-- TODO: ... -->
        </section>
    </article>
</main>

<style>
    :global(html, body, #app) {
        width: 100%;
        height: 100%;
    }
</style>
