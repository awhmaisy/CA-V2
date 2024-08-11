<script>
    import '/app.css';
</script>

<nav class="navbar">
    <div class="nav-left">
        <div class="search-icon">🔍</div>
        <a href="#">neue shit</a>
        <div class="more-dropdown">
            <a href="#" class="more-link">collections</a>
            <div class="dropdown-content">
                <a href="#">Page 1</a>
                <a href="#">Page 2</a>
                <a href="#">Page 3</a>
                <a href="#">Page 4</a>
            </div>
        </div>
    </div>
    <img src="/ca-heritage2.png" style="max-width: 130px; padding: 20px;" class="logo">
    <div class="nav-right">
        <a href="#">account</a>
        <a href="#">cart [1]</a>
    </div>
</nav>

<style>
.navbar {
    height: 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px; 
    background-color: white; 
    border-bottom: 1px solid #000; 
    position: relative; 
    justify-items: center;
}

.nav-left {
    display: flex;
    align-items: center;
}

.nav-left a {
    margin: 0 15px; /* Spacing between items */
    text-decoration: none; /* Remove underline */
    color: black; /* Text color */
}

.search-icon {
    margin-right: 15px; /* Spacing for the search icon */
}

.logo {
    position: absolute; /* Position absolute to center it */
    left: 50%; /* Move to the center */
    transform: translateX(-50%); /* Adjust for its own width */
    font-weight: bold; /* Style for the logo */
}

.nav-right {
    display: flex;
    align-items: center;
}

.nav-right a {
    margin-left: 15px; /* Spacing between account and cart */
}

.more-dropdown {
    position: relative;
}

.more-link {
    cursor: pointer; /* Change cursor to pointer */
}

.dropdown-content {
    display: none; /* Hide dropdown by default */
    position: absolute;
    background-color: white;
    min-width: 160px; /* Width of dropdown */
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
}

.more-dropdown:hover .dropdown-content {
    display: block; /* Show dropdown on hover */
}

.dropdown-content a {
    display: block; /* Make links block elements */
    padding: 10px; /* Add padding */
    margin-left: 0px; /* Add padding */
    margin-right: 0px; /* Add padding */
    color: black; /* Text color */
    text-decoration: none; /* Remove underline */
}

.dropdown-content a:hover {
    background-color: #f1f1f1; /* Change background on hover */
}
</style>