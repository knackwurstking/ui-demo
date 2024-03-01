<script>
    import { UI } from "ui";
</script>

<UI.FlexGrid.Root class="has-border" style="padding: 0.5em;" gap=".25em">
    <UI.FlexGrid.Row style="height: 5em;" gap="1em">
        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R1C1
        </UI.FlexGrid.Col>

        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R1C2
        </UI.FlexGrid.Col>

        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R1C3
        </UI.FlexGrid.Col>
    </UI.FlexGrid.Row>

    <UI.FlexGrid.Row style="height: 5em;">
        <UI.FlexGrid.Col
            class="has-border flex align-center justify-center"
            flex="2"
        >
            R2C1
        </UI.FlexGrid.Col>

        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R2C2
        </UI.FlexGrid.Col>

        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R2C3
        </UI.FlexGrid.Col>
    </UI.FlexGrid.Row>

    <UI.FlexGrid.Row style="height: 5em;">
        <UI.FlexGrid.Col
            class="has-border flex align-center justify-center"
            flex="0.5"
        >
            R3C1
        </UI.FlexGrid.Col>

        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R3C2
        </UI.FlexGrid.Col>

        <UI.FlexGrid.Col class="has-border flex align-center justify-center">
            R3C3
        </UI.FlexGrid.Col>
    </UI.FlexGrid.Row>
</UI.FlexGrid.Root>
