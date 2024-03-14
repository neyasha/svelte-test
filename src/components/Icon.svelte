<script>
    export let name;
    const icons = [
        {
            name: "check-mark",
        },
        {
            name: "delete",
        },
    ];
    let icon = icons.find((item) => item.name === name);
</script>
    