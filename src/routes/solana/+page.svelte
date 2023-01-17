<script lang=ts>
	import * as sol from '@solana/web3.js'
	import { cluster, connectedCluster } from "$lib/stores";
    import GetParsedAccountData from '$lib/components/GetParsedAccountData.svelte';
    import SetCluster from '$lib/components/SetCluster.svelte';

</script>

<svelte:head>
	<title>Metacamp</title>
</svelte:head>

<section class="w-full h-screen font-main">
	<div>
		<div class="flex m-4 mb-12 justify-center">
			<SetCluster />
		</div>
		<div class="flex m-4 mb-12 justify-center">
			<GetParsedAccountData />
		</div>
	</div>
</section>