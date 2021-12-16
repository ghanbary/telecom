<script>
    let count = 0;

    function increment() {
        return count++
    }

</script>

<div class="main">
    <h1 class="title">this is amazing sveltekit app</h1>
    <h3>Counter: <span class="counter">{count}</span></h3>
    <a href='/about'>go to about</a>
    <button on:click={increment}>Increment</button>
</div>

<style lang="postcss">

    .main {
        @apply max-w-screen-lg p-10 mx-auto;
    }

    .counter {
        @apply text-cyan-300 font-bold;
    }

    button {
        @apply py-3 px-4 text-white rounded bg-cyan-500;
    }

    .title {
        @apply text-2xl text-center mt-10 font-semibold;
    }
</style>