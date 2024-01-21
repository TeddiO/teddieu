<script>
    import { page } from "$app/stores";
    const d = new Date().getFullYear();
</script>

<svelte:head>
    <title>Well that's awkward, we found an error.</title>
</svelte:head>

<div class="container">
    <p>{$page.status}</p>
    <p id="shrug">¯\_(ツ)_/¯</p>
    <p>{$page.error.message}</p>
</div>

<p id="copyright">Background Image © {d} Chris Charlesworth</p>

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
        font-size: 4.5rem;
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

    #copyright {
        position: absolute;
        bottom: 0;
        font-size: 0.5rem;
        color: rgba(255, 255, 255, 0.8);
        font-family: "Roboto", sans-serif;
        left: 50%;
        transform: translateX(-50%);
    }
</style>
