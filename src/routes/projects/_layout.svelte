<script>
    export let segment;
</script>

<h2 class:active={segment === 'previous'}>pasdf</h2>

<style>

    .active {
        transform: scale(2);
    }

    h2 {
        display: flex;
        background-color: green;
    }

    .submenu {
        display: flex;
        justify-content: space-between;
        margin-bottom: 1em;
    }
</style>

<div class="submenu">
	<a class:active={segment === 'previous'} href="projects/previous">Previous</a>
	<a href="projects/next">Next</a>
</div>

<slot></slot>