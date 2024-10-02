<script>
    import { goto } from '$app/navigation';
    import nickimg from '$lib/images/nick.png'
    import mattimg from '$lib/images/matt.png'
</script>

<svelte:head>
    <title>Our Team</title>
    <meta name="description" content="Innovative Technology Solutions by TraceValley" />
</svelte:head>

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lora:700&display=swap">

<main>
    <section class="hero">
        <h1>Our Team</h1>
    </section>

    <section class="grid-container">
        <div class="grid-item">
            <h2>Nick</h2>
            <img src={nickimg} alt="Nick" />
            <p>The best engineer of all time way better than this guy on my right</p>
        </div>
        <div class="grid-item">
            <h2>Matt</h2>
            <img src={mattimg} alt="Matt" />
            <p>im dumb engineer</p>
        </div>
        <div class="grid-item">
            <h2>Coming Soon</h2>
            <p>...</p>
        </div>
        <div class="grid-item">
            <h2>Coming Soon</h2>
            <p>...</p>
        </div>
    </section>
</main>

<style>
    main {
        font-family: var(--font-body);
        padding: 2rem;
        max-width: 1200px;
        margin: 0 auto;
        text-align: center;
    }

    .hero h1 {
        font-size: 2.5rem;
        margin-bottom: 2rem;
        font-weight: bold;
    }

    .grid-container {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 2rem;
        justify-items: center;
    }

    .grid-item {
        background: rgba(30, 30, 30, 0.7); /* Dark gray glassy effect */
        backdrop-filter: blur(10px);
        border-radius: 15px;
        padding: 2rem;
        width: 100%;
        max-width: 400px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .grid-item:hover {
        transform: translateY(-10px);
        box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
    }

    .grid-item h2 {
        font-size: 1.5rem;
        margin-bottom: 1rem;
        color: #fff; /* White font for titles */
        font-weight: bold;
    }

    .grid-item img {
        width: 100%;
        height: auto;
        border-radius: 10px;
        margin-bottom: 1rem;
    }

    .grid-item p {
        font-size: 1rem;
        color: #fff; /* White font for paragraphs */
    }
</style>