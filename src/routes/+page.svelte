<script>
    import octocat from "$lib/github-mark-white-c.png";
    import steamicon from "$lib/steamworks-steam-logo.png";
    import instalogo from "$lib/instagramlogo.png";
</script>

<div class="container">
    <a
        href="https://github.com/TeddiO"
        target="_blank"
        rel="noopener noreferrer"
    >
        <img class="icon" src={octocat} alt="Github Profile" />
    </a>
    <a
        href="https://steamcommunity.com/id/0x740x650x640x640x69/"
        target="_blank"
        rel="noopener noreferrer"
    >
        <img class="icon" src={steamicon} alt="Steam Profile" />
    </a>

    <a
        href="https://www.instagram.com/i_am__teddi/"
        target="_blank"
        rel="noopener noreferrer"
    >
        <img class="icon" src={instalogo} alt="Steam Profile" />
    </a>
</div>

<style>
    :global(body) {
        background-image: url($lib/dji_0321.webp);
        background-repeat: no-repeat;
        background-size: cover;
        background-blend-mode: darken;
        background-color: rgba(0, 0, 0, 0.4);
        overflow-y: hidden;
    }

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
    }

    .icon {
        margin: 0 10px;
        width: 8vh;
        height: 8vh;
    }
</style>
