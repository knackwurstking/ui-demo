<script>
    import BackIcon from "svelte-material-icons/ArrowLeft.svelte";
    import SettingsIcon from "svelte-material-icons/FileSettings.svelte";
    import TrashIcon from "svelte-material-icons/TrashCanOutline.svelte";
    import { UI } from "ui";
</script>

<UI.Button.Root color="primary">Primary</UI.Button.Root>
<UI.Button.Root color="secondary">Secondary</UI.Button.Root>
<UI.Button.Root color="destructive">Destructive</UI.Button.Root>

<br />
<br />

<UI.Button.Root color="primary" variant="outline">Primary</UI.Button.Root>
<UI.Button.Root color="secondary" variant="outline">Secondary</UI.Button.Root>
<UI.Button.Root color="destructive" variant="outline">
    Destructive
</UI.Button.Root>

<br />
<br />

<UI.Button.Root color="primary" variant="ghost">Primary</UI.Button.Root>
<UI.Button.Root color="secondary" variant="ghost">Secondary</UI.Button.Root>
<UI.Button.Root color="destructive" variant="ghost">Destructive</UI.Button.Root>

<br />
<br />

<UI.Button.Icon ghost><SettingsIcon /></UI.Button.Icon>

<UI.Button.Icon color="destructive" ghost>
    <TrashIcon />
</UI.Button.Icon>

<UI.Button.Icon color="secondary"><BackIcon /></UI.Button.Icon>
