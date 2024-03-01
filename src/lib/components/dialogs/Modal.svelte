<script>
    import { UI } from "ui";

    export let fullscreen = false;

    /** @type {UI.Dialog.Root} */
    let dialog;

    export function open() {
        dialog.showModal();
    }

    export function close() {
        dialog.close();
    }
</script>

<UI.Dialog.Root bind:this={dialog} {fullscreen}>
    <UI.Dialog.Header title="Dialog Example" on:close={() => close()} />

    <section>
        <UI.Text.Primary>Content here ....</UI.Text.Primary>
    </section>

    <UI.Dialog.Footer>
        <UI.Button.Root
            variant="full"
            color="secondary"
            on:click={() => {
                dialog.close();
            }}>Cancel</UI.Button.Root
        >
    </UI.Dialog.Footer>
</UI.Dialog.Root>
