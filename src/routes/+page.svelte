<script>
	import { goto } from "$app/navigation";
</script>

<svelte:head>
    <title>TraceValley</title>
    <meta name="description" content="Innovative Technology Solutions by TraceValley" />
</svelte:head>

<main>
    <section class="hero">
        <h1>TraceValley</h1>
        <p>Welcome to the Future</p>
		<button on:click={() => goto('/OurMission')}>Learn More</button>
    </section>

    <!-- Add your other sections like About, Services, Contact here -->
</main>

<style>
	main {
		font-family: var(--font-body);
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
		margin: 0;
	}

	h1 {
		width: 100%;
		font-weight: bold;
		font-size: 5rem;
		margin: 0;
	}

	p {
		font-style: italic;
		font-size: 1.3rem;
		margin: 0;
	}

	button {
		padding: 10px 20px;
        background-color: #B80000;
        color: white;
        border: none;
        border-radius: 7px;
        cursor: pointer;
        margin-top: 20px; /* Space between text and button */
	}

	button:hover {
		background-color: #FF9800;
	}
</style>
