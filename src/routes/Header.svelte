<script>
	import { page } from '$app/stores';
	import {goto} from '$app/navigation';

</script>

<header>


	<nav>
		
		<ul>
				<button on:click={()=>goto('/')} >Introduction</button>
				
				<button on:click={()=>goto('/arrays')} >Arrays</button>

				<button on:click={()=>goto('/score')}>Score</button>
		</ul>
	</nav>


</header>

<slot></slot>