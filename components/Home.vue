<template>
    <div id="wrap-banner">
        <v-toolbar dark flat class="transparent" fixed>
            <v-spacer></v-spacer>
            <v-toolbar-side-icon class="hidden-md-and-up"></v-toolbar-side-icon>
            <v-toolbar-items class="hidden-sm-and-down menu-items">
                <v-btn flat>Home</v-btn>
                <v-btn flat>About</v-btn>
                <v-btn flat>Web Crawling</v-btn>
                <v-btn flat>Web Development</v-btn>
                <v-btn flat>Contact</v-btn>
            </v-toolbar-items>
        </v-toolbar>
            <div class="main-section">
                <div class="title">
                    <h2>Mega Bang</h2>
                </div>
            </div>
            <vue-particles color="#dedede" :particleOpacity="1" :particlesNumber="80" shapeType="circle" :particleSize="4" linesColor="#dedede"
                :linesWidth="1" :lineLinked="true" :lineOpacity="0.4" :linesDistance="150" :moveSpeed="3" :hoverEffect="true"
                hoverMode="grab" :clickEffect="true" clickMode="push">
            </vue-particles>
    </div>

</template>

<style lang="css" scoped>
    #particles-js {
        background-color: black;
        height: 100vh;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    #wrap-banner {
        position: relative;
    }

    .main-section {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        -webkit-align-items: center;
        -ms-flex-align: center;
        align-items: center;
        display: -webkit-flex;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .title>h2 {
        font-size: 7rem;
        font-weight: bold;
    }
</style>