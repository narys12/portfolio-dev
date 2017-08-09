<template>
    <div>
        <v-toolbar flat class="transparent" fixed>
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
        <vue-particles color="#dedede"  class="bg" :particleOpacity="1" :particlesNumber="80" shapeType="circle" :particleSize="8"
            linesColor="#dedede" :linesWidth="1" :lineLinked="true" :lineOpacity="0.4" :linesDistance="150" :moveSpeed="3" :hoverEffect="true"
            hoverMode="grab" :clickEffect="true" clickMode="push">
        </vue-particles>
    </div>

</template>

<style lang="css" scoped>
    .bg {
        background-image: url("http://newboundnetwork.com/wp-content/uploads/2014/04/icon-feed-bot.png");
        height: 100vh;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>