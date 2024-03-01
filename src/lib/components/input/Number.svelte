<script>
    import { UI } from "ui";
</script>

<UI.Text.Label primary="Number" secondary="UI.Input.Number ...">
    <UI.Input.Number
        title="Age"
        min={0}
        max={150}
        on:change={() => console.debug("number:change")}
        on:input={() => console.debug("number:input")}
    />
</UI.Text.Label>
