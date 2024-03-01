<script>
    import { onMount } from "svelte";

    import BackIcon from "svelte-material-icons/ArrowLeft.svelte";
    import SaveIcon from "svelte-material-icons/ContentSave.svelte";

    import { UI } from "ui";
</script>

<div
    style="position: relative; height:10em; border-bottom: none;"
    class="is-max-width has-border"
>
    <UI.TopAppBar.Root>
        <svelte:fragment slot="left">
            <UI.Button.Icon ghost>
                <BackIcon />
            </UI.Button.Icon>
        </svelte:fragment>

        <svelte:fragment slot="center">
            <h3>Settings</h3>
        </svelte:fragment>

        <svelte:fragment slot="right">
            <UI.Button.Icon ghost>
                <SaveIcon />
            </UI.Button.Icon>
        </svelte:fragment>
    </UI.TopAppBar.Root>
</div>
