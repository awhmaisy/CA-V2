<script>
    import { onMount } from 'svelte';
    let lastUpdated = '';

    onMount(async () => {
        const response = await fetch('/lastDeployed.json');
        const data = await response.json();
        lastUpdated = data.lastDeployed || new Date().toLocaleString();
    });
</script>

<footer>
    <p>Last Updated: {lastUpdated}</p>
    <p>©2001 Microsoft Corporation. All rights reserved. <a href="#">Terms of Use</a></p>
    <p>
        <a href="#">Text-only Home Page</a> | 
        <a href="#">Disability/accessibility</a> | 
        <a href="#">Contact Us</a> | 
        <a href="#">Privacy Statement</a>
    </p>
</footer>
<style>
footer {
    text-align: center; /* Center the text */
    padding: 10px; /* Add some padding */
}
footer a {
    color: blue; /* Link color */
    text-decoration: underline; /* Underline links */
}
</style>