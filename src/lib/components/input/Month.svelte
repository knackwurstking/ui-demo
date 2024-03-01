<script>
    import "ui/main.min.css";

    import { UI } from "ui";
</script>

<UI.Text.Label primary="Month" secondary="UI.Input.Month ...">
    <UI.Input.Month
        title="Pick a Month"
        on:change={() => console.debug("month:change")}
        on:input={() => console.debug("month:input")}
    />
</UI.Text.Label>
