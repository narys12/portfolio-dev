<template>
    <div class="main-section">
        <v-toolbar dark flat class="transparent" fixed>
            <v-spacer></v-spacer>
            <v-toolbar-side-icon class="hidden-md-and-up"></v-toolbar-side-icon>
            <v-toolbar-items class="hidden-sm-and-down">
                <v-btn flat>Home</v-btn>
                <v-btn flat>About</v-btn>
                <v-btn flat>Web Crawling</v-btn>
                <v-btn flat>Web Development</v-btn>
                <v-btn flat>Contact</v-btn>
            </v-toolbar-items>
        </v-toolbar>
        <vue-particles color="#dedede" class="bg" :particleOpacity="1" :particlesNumber="80" shapeType="circle" :particleSize="4"
            linesColor="#dedede" :linesWidth="1" :lineLinked="true" :lineOpacity="0.4" :linesDistance="150" :moveSpeed="3" :hoverEffect="true"
            hoverMode="grab" :clickEffect="true" clickMode="push">
        </vue-particles>
    </div>

</template>

<style lang="css" scoped>
    .bg {
        background-color: black;
        height: 100vh;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    .main-title {
        margin: auto;
        padding: 0 1rem;
        color: #fff;
        z-index: 999;
        position: relative;
        top: 600px;
    }

    .main-title h2 {
        font-size: 7rem;
        font-family: 'Teko', sans-serif;
        text-shadow: 8px 8px #000000;
        text-transform: uppercase;
        @media (max-width: 767px) {
            font-size: 3rem;
        }
    }

    .main-title p.subtitle {
        font-size: 1.7rem;
        margin: 0;
        @media (max-width: 767px) {
            font-size: 1rem;
        }
    }
</style>