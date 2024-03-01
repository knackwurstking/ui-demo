<script>
    import { UI } from "ui";

    import * as Dialogs from "./dialogs";

    /** @type {Dialogs.Root} */
    let dialog;
    /** @type {Dialogs.Modal} */
    let dialogModal;
    let fullscreen = false;
</script>

<UI.Button.Root
    color="secondary"
    on:click={() => {
        fullscreen = false;
        dialog.open();
    }}
>
    <!-- TODO: Needs to draggable (icon top left?) -->
    Normal (Work in Progress)
</UI.Button.Root>

<UI.Button.Root
    on:click={() => {
        fullscreen = false;
        dialogModal.open();
    }}
>
    Modal
</UI.Button.Root>

<br />
<br />

<UI.Button.Root
    color="secondary"
    on:click={() => {
        fullscreen = true;
        dialog.open();
    }}
>
    Normal Fullscreen
</UI.Button.Root>

<UI.Button.Root
    on:click={() => {
        fullscreen = true;
        dialogModal.open();
    }}
>
    Modal Fullscreen
</UI.Button.Root>

<Dialogs.Root bind:this={dialog} {fullscreen} />
<Dialogs.Modal bind:this={dialogModal} {fullscreen} />
