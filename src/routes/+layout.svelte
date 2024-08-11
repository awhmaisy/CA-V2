<script>
    import Navigation from '$lib/Navigation.svelte';
    import Footer from '$lib/Footer.svelte'; 
    import '/app.css';
</script>

<Navigation />
<slot />
<div class="divider"></div> 
<Footer />

<style>
    .divider {
        height: 1px;
        background-color: #000;
        margin: 20px 0; 
    }
    </style>