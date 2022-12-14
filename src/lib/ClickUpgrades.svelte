<script>
    import {clickPower, cookies} from "./stores.js";

    let upgradeCost = 50;

    function upgrade() {
        if ($cookies >= upgradeCost) {
            $clickPower += 1;
            $cookies -= upgradeCost;
            upgradeCost *= 1.17;
        }
    }
</script>

<button on:click={upgrade}>Upgrade click power</button>
{upgradeCost.toFixed(0)}
