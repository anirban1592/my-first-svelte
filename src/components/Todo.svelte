<script>
    let todo = "";
    let todos = [];

    const handleAdd = () => {
        if (todo.length != 0) {
            todos = [...todos, todo];
            todo = "";
        } else {
            alert("Please enter atleast 1 todo");
        }
    };
</script>

<div class="todo">
    <input type="text" bind:value={todo} />
    <button on:click={handleAdd}>Add todo</button>
</div>
<div class="container">
    <div class="todo-list">
        <ul>
            {#each todos as todo}
                <li>{todo}</li>
            {/each}
        </ul>
    </div>
</div>

<style>
    input {
        margin: 20px;
        max-width: 350px;
        width: 300px;
        height: 40px;
        border: solid;
        background-color: beige;
        font-size: 25px;
        border-radius: 15px;
        border-color: black;
        box-shadow: 1px 2px;
    }
    button {
        margin: 20px;
        width: 150px;
        border-color: azure;
        border-radius: 15px;
        box-shadow: 2px 1px;
        font-style: italic;
        font-size: 20px;
    }
    .todo {
        display: flex;
        justify-content: center;
    }
    .todo-list li {
        font-size: 40px;
    }
    .container ul {
        display: flex;
        flex-flow: column wrap;
        align-items: self-start;
        width: 500px;
        height: 500px;
        margin-left: 650px;
        max-width: 500px;
    }
    li:hover {
        font-size: 40px;
    }
</style>
