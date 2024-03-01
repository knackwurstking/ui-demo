<script>
    import { UI } from "ui";

    import Buttons from "./lib/components/Buttons.svelte";
    import Card from "./lib/components/Card.svelte";
    import Dialog from "./lib/components/Dialog.svelte";
    import Drawer from "./lib/components/Drawer.svelte";
    import FlexGrid from "./lib/components/FlexGrid.svelte";
    import * as Input from "./lib/components/input";
    import Spinner from "./lib/components/Spinner.svelte";
    import * as Text from "./lib/components/text";
    import ThemePicker from "./lib/components/ThemePicker.svelte";
    import TopAppBar from "./lib/components/TopAppBar.svelte";

    let drawerOpen = false;
</script>

<UI.Theme.Root auto />

<main class="is-max ui-container flex column align-center">
    <article class="is-max-width">
        <h1>Buttons</h1>

        <section>
            <Buttons />
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Card</h1>

        <section>
            <Card />
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Dialog</h1>

        <section>
            <Dialog />
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Drawer</h1>

        <section>
            <UI.Button.Root
                on:click={() => {
                    drawerOpen = true;
                }}
            >
                Open Drawer
            </UI.Button.Root>
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>Flex Grid</h1>

        <section>
            <FlexGrid />
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
            <ThemePicker />
        </section>

        <hr />
    </article>

    <article class="is-max-width">
        <h1>(Top) App Bar</h1>

        <section>
            <TopAppBar />
        </section>
    </article>

    <Drawer bind:open={drawerOpen} />
</main>

<style>
    :global(html, body, #app) {
        width: 100%;
        height: 100%;
    }
</style>
