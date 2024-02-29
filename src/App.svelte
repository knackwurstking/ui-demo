<script>
    import "ui/main.min.css";

    import { UI } from "ui";
</script>

<UI.Theme.Root auto />

<main class="is-max ui-container flex column align-center">
    <article class="is-max-width">
        <h1>Input Elements</h1>

        <section>
            <UI.Text.Label
                primary="Input Slider"
                secondary="UI.Input.Slider min={0} max={100} value={50}"
                row
            >
                <UI.Input.Slider
                    style="width: 50%;"
                    min={0}
                    max={100}
                    value={50}
                />
            </UI.Text.Label>
        </section>
    </article>
</main>

<style>
    :global(html, body, #app) {
        width: 100%;
        height: 100%;
    }
</style>
