<script>
    import { page } from "$app/stores";
    $: isActive = $page.path === $$props.href;
</script>

<a {...$$props} class:active={isActive}>
    <slot />
</a>