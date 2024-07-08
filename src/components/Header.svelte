<script>
    export let y;

    let tabs = [
        {name: 'Projects', '#projects'},
        {name: 'About Me', '#About Me'},
    ]
</script>

<header>
    <h1>
        <b>David</b> Sanchez
    </h1>
    <div class="">
        {#each tabs as tab, index}
            <a>
                <p>{tab.name}</p>
            </a>
        {/each}
    </div>
</header>