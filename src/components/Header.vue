<template>
    <div class="header-content">
        <div>
            <img src="/pixel_background_gif.gif" alt="" class="background-image">
        </div>
        <div id="nav-bar">
            <nav>
                <div><a href="#home" @click.prevent="scrollToSection('home')">Home</a></div>
                <div><a href="#about" @click.prevent="scrollToSection('about')">About</a></div>
                <div><a href="#projects" @click.prevent="scrollToSection('projects')">Projects</a></div>
                <div><a href="#contact" @click.prevent="scrollToSection('contact')">Contact</a></div>
            </nav>
        </div>
        <div id="content">
            <h1 id="text">Hi, I'm
                <br>
                <span>Full Name</span>
            </h1>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Header',
    methods: {
        scrollToSection(sectionId) {
            const section = document.getElementById(sectionId);
            if (section) {
                section.scrollIntoView({ behavior: 'smooth' });
            }
        }
    }
}
</script>

<style>
.header-content {
    position: relative;
    width: 100vw;
    height: 100vh;
    /* background-image: url('/pixel_background_gif.gif'); */
    /* background-size: cover;
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat; */
    /* color: white; */
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.background-image {
    position: absolute;
    width: 100%;
    height: 100vh;
    top: 0;
    left: 0;
    object-fit: cover;
    z-index: -1;
}

#nav-bar {
    position: absolute;
    top: 0;
    width: 100%;
}

nav {
    display: flex;
    justify-content: center;
    gap: 30px;
}

nav div {
    display: flex;
}

nav a {
    text-decoration: none;
    color: white;
    font-size: 1.2rem;
    padding: 10px 20px;
    transition: color 0.3s ease;
}

nav a:hover {
    color: #ff5733;
    text-decoration: underline;
}

#content {
    position: relative;
    top: 50%;
    transform: translateY(-50%);
}

#text {
    font-size: 50px;
}

/* Responsive adjustments */
@media (max-width: 768px) {
    .header-content {
        background-size: contain;
        background-position: top;
    }

    .background-image {
        object-fit: contain;
    }
}

@media (max-width: 480px) {
    .header-content {
        background-size: contain;
        background-position: top;
    }

    .background-image {
        object-fit: contain;
    }
}
</style>