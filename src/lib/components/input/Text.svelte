<script>
    import { UI } from "ui";
</script>

<UI.Text.Label primary="Number" secondary="UI.Input.Number ...">
    <UI.Input.Text
        title="Alias"
        value="knackwurstking"
        on:change={() => console.debug("text:change")}
        on:input={() => console.debug("text:input")}
    />
</UI.Text.Label>
