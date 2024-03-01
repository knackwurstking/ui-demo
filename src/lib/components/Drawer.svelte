<script>
    import { UI } from "ui";

    export let open = true;
</script>

<UI.Drawer.Root bind:open>
    <UI.Drawer.Group>
        <!-- NOTE: slot "title" not needed here -->
        <UI.Drawer.GroupTitle slot="title">Group Title</UI.Drawer.GroupTitle>

        <UI.Drawer.GroupItem>
            <UI.Button.Root
                class="is-max-width"
                color="primary"
                variant="full"
                on:click={() => (open = false)}
            >
                Click me!
            </UI.Button.Root>
        </UI.Drawer.GroupItem>

        <UI.Drawer.GroupItem>
            <UI.Text.Label
                primary="Group item..."
                secondary="...can be anything"
            />
        </UI.Drawer.GroupItem>

        <UI.Drawer.GroupItem>
            <hr class="is-max-width" />
        </UI.Drawer.GroupItem>
    </UI.Drawer.Group>
</UI.Drawer.Root>
