<template>
    <nav class="navbar has-shadow" role="navigation" aria-label="main navigation">
        <div class="container">
            <div class="navbar-brand">
                <a class="navbar-item" href="https://leamsigc.git">
                    Leamsigc
                </a>

                <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false"  v-on:click='toggleNav'  v-bind:class="{ 'is-active': isActive }">
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                </a>
            </div>
            <div class="navbar-menu" v-on:click='toggleNav' v-bind:class="{'is-active':isActive}">
                <div class="navbar-end">
                    <a href="/" class="navbar-item">Home</a>
                    <a href="/" class="navbar-item">About</a>
                    <a href="/" class="navbar-item">Portfolio</a>
                    <a href="/" class="navbar-item">Contact</a>

                    <div class="navbar-item">
                        <div class="field">
                        <p class="control">
                        <a class="button is-warning is-outlined" href="https://github.com/jgthms/bulma/releases/download/0.7.1/bulma-0.7.1.zip">
                            <span class="icon">
                                <i class="fa fa-twitter"></i>
                            </span>
                            <span>Contact now</span>
                        </a>
                        </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "Nav",
        data: function (){
            return {
                isActive: false
            }
        },
        methods: {
            toggleNav:function () {
                this.isActive = !this.isActive
            }
        }
    };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped>
    @import '../mediaquerys' 
    .navbar 
        background-color: #383838
        a
            color: #c1c1c1
            padding: 0.5rem 1.75rem
            &:hover
                background-color: #383838
                color: gray
    .navbar-brand a 
        color: #fff
        font-weigth: 700
    .navbar-menu
        background: #333
</style>