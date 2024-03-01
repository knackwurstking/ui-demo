<script>
    import { UI } from "ui";

    /**
     * @type {import("ui/svelte/input/html-select").SelectItem[]}
     */
    const listItems = [
        { label: "List entry 1", value: "le1" },
        { label: "List entry 2", value: "le2" },
        { label: "List entry 3", value: "le3" },
        { label: "List entry 4", value: "le4" },
        { label: "List entry 5", value: "le5" },
    ];
</script>

<UI.Text.Label primary="HTMLSelect" secondary="UI.Input.HTMLSelect ...">
    <UI.Input.HTMLSelect
        items={listItems}
        selected={listItems[0] || null}
        on:change={() => console.debug("html-select:change")}
    />
</UI.Text.Label>
