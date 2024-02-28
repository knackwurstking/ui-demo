<script>
    import "ui/main.min.css";

    import { UI } from "ui";
</script>

<UI.Theme.Root auto />

<main class="is-max ui-container flex column align-center justify-center">
    <div style:width="10em">
        <UI.Input.Slider min={0} max={100} value={50} />
    </div>
</main>

<style>
    :global(html, body, #app) {
        width: 100%;
        height: 100%;
    }
</style>
