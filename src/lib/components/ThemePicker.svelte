<script>
    import { UI } from "ui";

    /**
     * @type {"dark" | "light" | null}
     */
    let mode = "dark";

    let auto = false;
    let title = "Dark Mode";
</script>

<UI.Theme.Root variant="zinc" {mode} {auto} />

<UI.FlexGrid.Root gap="1em">
    <UI.FlexGrid.Col>
        <UI.FlexGrid.Row gap="1em">
            <UI.Text.Primary>{title}</UI.Text.Primary>
        </UI.FlexGrid.Row>

        <UI.FlexGrid.Row gap="1em">
            <UI.Button.Root
                color="primary"
                on:click={() => {
                    mode = null;
                    auto = true;
                    title = "System Mode";
                }}
            >
                System
            </UI.Button.Root>

            <UI.Button.Root
                color="secondary"
                on:click={() => {
                    mode = "dark";
                    auto = false;
                    title = "Dark Mode";
                }}>Dark</UI.Button.Root
            >

            <UI.Button.Root
                color="secondary"
                on:click={() => {
                    mode = "light";
                    auto = false;
                    title = "Light Mode";
                }}>Light</UI.Button.Root
            >
        </UI.FlexGrid.Row>
    </UI.FlexGrid.Col>
</UI.FlexGrid.Root>
