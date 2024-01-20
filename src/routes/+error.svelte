<script>
    import { page } from "$app/stores";
</script>

<svelte:head>
    <title>Knocking about somewhere.</title>
</svelte:head>

<div class="container">
    <p>{$page.status}</p>
    <p id="shrug">¯\_(ツ)_/¯</p>
    <p>{$page.error.message}</p>
</div>

⠀

<style>
    :global(body) {
        background-image: url($lib/dji_0321.webp);
        background-repeat: no-repeat;
        background-size: cover;
        background-blend-mode: darken;
        background-color: rgba(0, 0, 0, 0.4);
        overflow-y: hidden;
        user-select: none;
    }

    #shrug {
        font-size: 7rem;
        color: white;
        margin-top: 5px;
        margin-bottom: 5px;
    }

    p {
        text-align: center;
        justify-content: center;
        color: white;
        font-size: 3rem;
        font-family: "Roboto", sans-serif;
    }

    .container {
        height: 100vh;
    }
</style>
