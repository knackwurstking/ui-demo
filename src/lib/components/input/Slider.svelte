<script>
    import "ui/main.min.css";

    import { UI } from "ui";
</script>

<UI.Text.Label
    primary="Slider"
    secondary="UI.Input.Slider min={0} max={100} value={50}"
    row
>
    <UI.Input.Slider style="width: 50%;" min={0} max={100} value={50} />
</UI.Text.Label>
