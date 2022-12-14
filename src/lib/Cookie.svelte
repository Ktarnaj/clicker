<script>
    import {clickPower, cookies} from "./stores.js";

    function increment() {
        cookies.update(n => n + $clickPower);
    }
</script>

<button on:click={increment}>
    +
</button>