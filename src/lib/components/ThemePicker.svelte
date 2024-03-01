<script>
    import { UI } from "ui";

    /**
     * @type {"dark" | "light" | null}
     */
    let mode = "dark";

    let auto = false;
    let currentMode = "Dark";
</script>

<UI.Theme.Root variant="zinc" {mode} {auto} />

<UI.FlexGrid.Root gap=".5em">
    <UI.FlexGrid.Row>
        <UI.Text.Primary style="font-weight: 100;">
            Current Mode: <span style="font-weight: bold;">{currentMode}</span>
        </UI.Text.Primary>
    </UI.FlexGrid.Row>

    <UI.FlexGrid.Row gap=".25em">
        <UI.Button.Root
            color="primary"
            on:click={() => {
                mode = null;
                auto = true;
                currentMode = "System";
            }}
        >
            System
        </UI.Button.Root>

        <UI.Button.Root
            color="secondary"
            on:click={() => {
                mode = "dark";
                auto = false;
                currentMode = "Dark";
            }}>Dark</UI.Button.Root
        >

        <UI.Button.Root
            color="secondary"
            on:click={() => {
                mode = "light";
                auto = false;
                currentMode = "Light";
            }}>Light</UI.Button.Root
        >
    </UI.FlexGrid.Row>
</UI.FlexGrid.Root>
