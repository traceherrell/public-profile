<script>
    import history from "./history";
</script>

<svelte:head>
    <title>Work History</title>
</svelte:head>

<section>
    <div class="container">
        <h2 class="heading">Work History</h2>
        {#each history as h}
            <h5>
                {h.title}, <a href = {h.urls[0]}> <span style="font-style: italic;">{h.company}</span></a>
                <span style="float:right">{h.start} - {h.end} </span>
            </h5>
            <ul>
                {#each h.highlights as i}
                    <li>{i}</li>
                {/each}
            </ul>
        {/each}
    </div>
</section>

<style>
    .heading {
        margin-bottom: 50px;
    }
</style>
