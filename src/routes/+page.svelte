<script>
    import Todo from "../components/Todo.svelte";
</script>

<h1>Welcome to My Todo App</h1>
<Todo />

<style>
    h1 {
        margin: auto;
        width: 60%;
        border: 3px;
        padding: 80px 0;
        text-align: center;
    }

    :global(body) {
        background-color: cadetblue;
    }
</style>
