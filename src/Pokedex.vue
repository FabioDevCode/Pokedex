<template>
    <header>
        <img src="./assets/pokedex_title white.png" alt="logo pokedex">
    </header>

    <main>
        <div id="bloc_left" class="bloc">
            <div class="border_screen">
                <div class="screen_left">

                </div>
            </div>

            <div class="bottom_bloc">
                <button class="random"></button>

                <div class="screen_down"></div>

                <div class="bloc_direction">
                    <div class="btn_dir"></div>
                </div>
            </div>
        </div>
        <!-- SEPERATION - Haut Gauche / Bas Droite -->
        <div id="bloc_right" class="bloc">
            <div class="screen_right"></div>

            <div class="bloc_btn_blue">
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
                    <button></button>
            </div>

            <div class="bloc_btn_grey">
                <button></button>
                <button></button>
            </div>

            <div class="bloc_screen">
                <div></div>
                <div></div>
            </div>
        </div>
    </main>


    <footer>
        <p>Coded by <a target="_blank" href="https://www.linkedin.com/in/fabio-ramoslopes/">Fabio R. LOPES</a></p>
    </footer>
</template>


<script>
    import pokemon from "@/assets/data/pokemon.js";

    export default {
        name: 'Pokedex',
        data() {
            return {
                pokemon: [],
            }
        },
        mounted() {
            this.getAllPokemon();
        },
        methods: {
            getAllPokemon() {
                this.pokemon = pokemon;
            }

        },
    }
</script>


<style>
    /*------RESET------*/
    *, ::before, ::after {
        box-sizing: border-box;
        padding: 0;
        margin: 0;
    }

    body {
        overflow-x: hidden;
        min-width: 375px;
        background-color: #AD4B46;
        color: #F3F3F3;
        font-family: Helvetica, sans-serif;
    }

    a {
        text-decoration: none;
        color: #F3F3F3;
    }

    button, input {
        border: none;
    }

    button:active {
        transform: scale(.95);
    }

    /* TEXTE
    font-family: 'Audiowide', cursive; */
    /* DESCRIPTION
    font-family: 'Major Mono Display', monospace; */

    /*------HEADER------*/
    header {
        margin: 35px auto;
        width: max-content;
    }

    header img {
        height: 50px;
        filter: drop-shadow(4px 4px 12px rgba(1, 1, 1, .5));
    }

    /*-------MAIN-------*/
    main {
        width: 900px;
        height: 620px;
        margin: 0 auto;
        display: flex;
        /* background-color: brown; */
    }
    main .bloc {
        position: relative;
        width: 450px;
        height: 620px;
    }
    .border_screen {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #D9D9D9;
        box-shadow: inset 8px 8px 20px rgba(255, 255, 255, .9),
                    inset -8px -8px 20px rgba(1, 1, 1, .5);
        width: 450px;
        height: 400px;
        border-radius: 10px 10px 10px 50px;
    }
    .screen_left {
        width: 350px;
        height: 280px;
        background-color: #333333;
        box-shadow: inset 4px 4px 15px rgba(1, 1, 1, .8);
        border-radius: 5px;
    }
    .screen_left, .screen_down, .screen_right {
        overflow-y: auto;
        overflow-x: hidden;
    }

    .bottom_bloc {
        height: 220px;
        width: 450px;
        display: flex;
    }
    .random {
        cursor: pointer;
        background-color: #222222;
        box-shadow: inset 2px 2px 8px rgba(243, 243, 243, .3),
                    inset -2px -2px 8px rgba(1, 1, 1, .8);
        height: 70px;
        width: 70px;
        border-radius: 70px;
        margin: 75px 0;
    }

    .screen_down {
        margin: 0 0 0 25px;
        align-self: flex-end;
        height: 100px;
        width: 180px;
        background-color: #333333;
        box-shadow: inset 4px 4px 8px rgba(1, 1, 1, .5);
        border-radius: 5px;
    }

    .bloc_direction {
        position: relative;
        margin: 0 0 0 25px;
        align-self: flex-end;
        height: 150px;
        width: 150px;
    }
    .bloc_direction .btn_dir {
        position: absolute;
        height: 150px;
        width: 150px;
        background-color: #222222;
    }

    /*------RIGHT------*/
    #bloc_right {
        padding-left: 100px;

    }
    .screen_right {
        width: 350px;
        height: 140px;
        background-color: #333333;
        box-shadow: inset 4px 4px 8px rgba(1, 1, 1, .5);
        border-radius: 5px;
        margin-top: 50px;
    }

    .bloc_btn_blue {
        width: 350px;
        height: 140px;
        margin-top: 40px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        background: radial-gradient(#853a36, transparent);
    }
    .bloc_btn_blue button {
        cursor: pointer;
        width: 65px;
        height: 65px;
        border-radius: 5px;
        margin: 0;
        background-color: #28ABFD;
        box-shadow: inset 2px 2px 8px rgba(243, 243, 243, .4),
                    inset -2px -2px 8px rgba(1, 1, 1, .4);
    }

    .bloc_btn_grey {
        height: 70px;
        width: 140px;
        margin-top: 40px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
    }
    .bloc_btn_grey button {
        cursor: pointer;
        width: 65px;
        height: 65px;
        border-radius: 5px;
        box-shadow: inset 2px 2px 8px rgba(243, 243, 243, .6),
                    inset -2px -2px 8px rgba(1, 1, 1, .6);
    }


    /*------FOOTER------*/
    footer {
        height: 100px;
        width: 310px;
        margin: 25px auto 0 auto;
        display: flex;
        font-family: 'Audiowide', cursive;
        justify-content: center;
        align-items: center;
    }
    footer a:active {
        color: #333333;
    }
    footer a:hover {
        color: #333333;
        text-shadow: 0 0 2px #333333;
    }

</style>