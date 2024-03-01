<script>
    import { UI } from "ui";
</script>

<UI.Text.Label
    primary="Slider"
    secondary="UI.Input.Slider min={0} max={100} value={50}"
>
    <UI.Input.Slider
        style="width: 50%;"
        min={0}
        max={100}
        value={50}
        on:change={() => console.debug("search:change")}
        on:input={() => console.debug("search:input")}
    />
</UI.Text.Label>
