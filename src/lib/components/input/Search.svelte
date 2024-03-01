<script>
    import { UI } from "ui";
</script>

<UI.Text.Label primary="Search" secondary="UI.Input.Search ...">
    <UI.Input.Search
        title="Search for some stuff here"
        placeholder="Search..."
        disableSubmit={false}
        on:submit={() => console.debug("search:submit")}
        on:change={() => console.debug("search:change")}
        on:input={() => console.debug("search:input")}
    />
</UI.Text.Label>
