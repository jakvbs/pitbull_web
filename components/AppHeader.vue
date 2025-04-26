<script setup lang="ts"></script>

<template>
    <nav class="navbar is-black py-0" role="navigation" aria-label="top bar">
        <div
            class="navbar-menu is-active"
            style="display: flex; width: 100%; align-items: stretch"
        >
            <!-- Align stretch -->
            <div class="navbar-start">
                <a class="navbar-item has-text-white">
                    <span class="icon mr-1"
                        ><i class="fas fa-map-marker-alt"></i
                    ></span>
                    <span>Nasze salony</span>
                </a>
            </div>

            <div
                class="navbar-item has-text-centered has-text-white is-hidden-touch"
                style="
                    flex-grow: 1;
                    line-height: 1.2;
                    display: flex;
                    align-items: center;
                    justify-content: center;
                "
            >
                <!-- Added flex centering -->
                <div class="is-flex is-flex-direction-column">
                    <span class="has-text-weight-bold is-size-7"
                        >KOLEKCJA WIOSNA/LATO 2025!</span
                    >
                    <span class="is-size-7">POKAŻ PRODUKTY!</span>
                </div>
            </div>

            <div class="navbar-end">
                <a class="navbar-item has-text-white">
                    <span class="icon mr-1"><i class="fas fa-user"></i></span>
                    <span>Moje konto</span>
                </a>
                <a class="navbar-item has-text-white">
                    <span class="icon mr-1">
                        <i class="fas fa-heart"></i>
                        <!-- Potential: Add a badge using Bulma's badge extension or custom CSS -->
                    </span>
                    <span>Lista życzeń</span>
                </a>
                <div class="navbar-item p-0">
                    <!-- Ensure item itself has no padding -->
                    <a class="button is-success has-text-white is-fullheight">
                        <!-- Removed is-light/is-small, added is-fullheight -->
                        <span class="icon"
                            ><i class="fas fa-shopping-cart"></i
                        ></span>
                        <span>Koszyk (0)</span>
                    </a>
                </div>
            </div>
        </div>
    </nav>
</template>

<style scoped>
.navbar {
    min-height: 44px; /* Adjusted height - match original image */
    align-items: stretch;
}

.navbar-menu {
    padding: 0;
    flex-grow: 1;
    align-items: stretch;
}

.navbar-item {
    display: flex;
    align-items: center;
    padding-top: 0;
    padding-bottom: 0;
}

.navbar-start,
.navbar-end {
    align-items: stretch;
}

/* Make button fill the navbar item height */
.navbar-item .button.is-fullheight {
    height: 100%;
    border-radius: 0; /* Remove radius for edge-to-edge look */
    padding-left: 1.5rem; /* Adjust padding as needed */
    padding-right: 1.5rem; /* Adjust padding as needed */
    font-size: 0.875rem; /* Match other item text size */
}

/* Ensure icons are vertically centered if needed */
.navbar-item .icon {
    display: inline-flex;
    align-items: center;
}

/* Reduce default space around icons slightly if needed */
.navbar-item .icon:not(:last-child) {
    margin-right: 0.25rem; /* Adjust spacing */
}
</style>
