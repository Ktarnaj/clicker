<script>
import {cookies} from "../lib/stores.js";
import Cookie from "../lib/Cookie.svelte";
import ClickUpgrades from "../lib/ClickUpgrades.svelte";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

{$cookies.toFixed(0)}

<Cookie></Cookie>
<ClickUpgrades></ClickUpgrades>