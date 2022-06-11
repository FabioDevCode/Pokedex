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
                <button class="select">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M438.6 105.4C451.1 117.9 451.1 138.1 438.6 150.6L182.6 406.6C170.1 419.1 149.9 419.1 137.4 406.6L9.372 278.6C-3.124 266.1-3.124 245.9 9.372 233.4C21.87 220.9 42.13 220.9 54.63 233.4L159.1 338.7L393.4 105.4C405.9 92.88 426.1 92.88 438.6 105.4H438.6z"/></svg>
                </button>

                <div class="screen_down"></div>

                <div class="bloc_direction">
                    <div class="btn_dir1"></div>
                    <div class="btn_dir2"></div>

                    <button class="up">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512"><path d="M27.66 224h264.7c24.6 0 36.89-29.78 19.54-47.12l-132.3-136.8c-5.406-5.406-12.47-8.107-19.53-8.107c-7.055 0-14.09 2.701-19.45 8.107L8.119 176.9C-9.229 194.2 3.055 224 27.66 224z"/></svg>
                    </button>
                    <button class="right">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 512"><path d="M118.6 105.4l128 127.1C252.9 239.6 256 247.8 256 255.1s-3.125 16.38-9.375 22.63l-128 127.1c-9.156 9.156-22.91 11.9-34.88 6.943S64 396.9 64 383.1V128c0-12.94 7.781-24.62 19.75-29.58S109.5 96.23 118.6 105.4z"/></svg>
                    </button>
                    <button class="down">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512"><path d="M310.6 246.6l-127.1 128C176.4 380.9 168.2 384 160 384s-16.38-3.125-22.63-9.375l-127.1-128C.2244 237.5-2.516 223.7 2.438 211.8S19.07 192 32 192h255.1c12.94 0 24.62 7.781 29.58 19.75S319.8 237.5 310.6 246.6z"/></svg>
                    </button>
                    <button class="left">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 512"><path d="M137.4 406.6l-128-127.1C3.125 272.4 0 264.2 0 255.1s3.125-16.38 9.375-22.63l128-127.1c9.156-9.156 22.91-11.9 34.88-6.943S192 115.1 192 128v255.1c0 12.94-7.781 24.62-19.75 29.58S146.5 415.8 137.4 406.6z"/></svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- SEPERATION - Haut Gauche / Bas Droite -->
        <div id="bloc_right" class="bloc">
            <div class="screen_right"></div>

            <div class="bloc_btn_blue">
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M0 96C0 78.33 14.33 64 32 64H416C433.7 64 448 78.33 448 96C448 113.7 433.7 128 416 128H32C14.33 128 0 113.7 0 96zM64 256C64 238.3 78.33 224 96 224H480C497.7 224 512 238.3 512 256C512 273.7 497.7 288 480 288H96C78.33 288 64 273.7 64 256zM416 448H32C14.33 448 0 433.7 0 416C0 398.3 14.33 384 32 384H416C433.7 384 448 398.3 448 416C448 433.7 433.7 448 416 448z"/></svg>
                </button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512"><path d="M412.6 182c-10.28-8.334-25.41-6.867-33.75 3.402c-8.406 10.24-6.906 25.35 3.375 33.74C393.5 228.4 400 241.8 400 255.1c0 14.17-6.5 27.59-17.81 36.83c-10.28 8.396-11.78 23.5-3.375 33.74c4.719 5.806 11.62 8.802 18.56 8.802c5.344 0 10.75-1.779 15.19-5.399C435.1 311.5 448 284.6 448 255.1S435.1 200.4 412.6 182zM473.1 108.2c-10.22-8.334-25.34-6.898-33.78 3.34c-8.406 10.24-6.906 25.35 3.344 33.74C476.6 172.1 496 213.3 496 255.1s-19.44 82.1-53.31 110.7c-10.25 8.396-11.75 23.5-3.344 33.74c4.75 5.775 11.62 8.771 18.56 8.771c5.375 0 10.75-1.779 15.22-5.431C518.2 366.9 544 313 544 255.1S518.2 145 473.1 108.2zM534.4 33.4c-10.22-8.334-25.34-6.867-33.78 3.34c-8.406 10.24-6.906 25.35 3.344 33.74C559.9 116.3 592 183.9 592 255.1s-32.09 139.7-88.06 185.5c-10.25 8.396-11.75 23.5-3.344 33.74C505.3 481 512.2 484 519.2 484c5.375 0 10.75-1.779 15.22-5.431C601.5 423.6 640 342.5 640 255.1S601.5 88.34 534.4 33.4zM301.2 34.98c-11.5-5.181-25.01-3.076-34.43 5.29L131.8 160.1H48c-26.51 0-48 21.48-48 47.96v95.92c0 26.48 21.49 47.96 48 47.96h83.84l134.9 119.8C272.7 477 280.3 479.8 288 479.8c4.438 0 8.959-.9314 13.16-2.835C312.7 471.8 320 460.4 320 447.9V64.12C320 51.55 312.7 40.13 301.2 34.98z"/></svg>
                </button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path d="M.1193 494.1c-1.125 9.5 6.312 17.87 15.94 17.87l32.06 .0635c8.125 0 15.21-5.833 16.21-13.83c.7501-4.875 1.869-11.17 3.494-18.17h312c1.625 6.875 2.904 13.31 3.529 18.18c1.125 7.1 7.84 13.94 15.97 13.82l32.46-.0625c9.625 0 17.12-8.374 15.99-17.87c-4.625-37.87-25.75-128.1-119.1-207.7c-17.5 12.37-36.98 24.37-58.48 35.49c6.25 4.625 11.56 9.405 17.06 14.15H159.7c21.25-18.12 47.03-35.63 78.65-51.38c172.1-85.5 203.7-218.8 209.5-266.7c1.125-9.5-6.297-17.88-15.92-17.88L399.6 .001c-8.125 0-14.84 5.832-15.96 13.83c-.7501 4.875-1.869 11.17-3.369 18.17H67.74C66.24 25 65.08 18.81 64.33 13.81C63.21 5.813 56.48-.124 48.36 .001L16.1 .1338c-9.625 0-17.09 8.354-15.96 17.85c5.125 42.87 31.29 153.8 159.9 238.1C31.55 340.3 5.245 451.2 .1193 494.1zM223.9 219.7C198.8 205.9 177.6 191.3 159.7 176h128.5C270.4 191.3 249 206.1 223.9 219.7zM355.1 96c-5.875 10.37-12.88 21.12-21 31.1H113.1c-8.25-10.87-15.3-21.63-21.05-32L355.1 96zM93 415.1c5.875-10.37 12.74-21.13 20.87-32h219.4c8.375 10.87 15.48 21.63 21.23 32H93z"/></svg>
                </button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512"><path d="M416 288h-95.1c-17.67 0-32 14.33-32 32s14.33 32 32 32H416c17.67 0 32-14.33 32-32S433.7 288 416 288zM352 416h-32c-17.67 0-32 14.33-32 32s14.33 32 32 32h32c17.67 0 31.1-14.33 31.1-32S369.7 416 352 416zM480 160h-159.1c-17.67 0-32 14.33-32 32s14.33 32 32 32H480c17.67 0 32-14.33 32-32S497.7 160 480 160zM544 32h-223.1c-17.67 0-32 14.33-32 32s14.33 32 32 32H544c17.67 0 32-14.33 32-32S561.7 32 544 32zM151.6 41.95c-12.12-13.26-35.06-13.26-47.19 0l-87.1 96.09C4.475 151.1 5.35 171.4 18.38 183.3c6.141 5.629 13.89 8.414 21.61 8.414c8.672 0 17.3-3.504 23.61-10.39L96 145.9v302C96 465.7 110.3 480 128 480s32-14.33 32-32.03V145.9L192.4 181.3C204.4 194.3 224.6 195.3 237.6 183.3c13.03-11.95 13.9-32.22 1.969-45.27L151.6 41.95z"/></svg>
                </button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><path d="M318 145.6c-3.812 8.75-12.45 14.41-22 14.41L224 160v272c0 44.13-35.89 80-80 80H32c-17.67 0-32-14.31-32-32s14.33-32 32-32h112C152.8 448 160 440.8 160 432V160L88 159.1c-9.547 0-18.19-5.656-22-14.41S63.92 126.7 70.41 119.7l104-112c9.498-10.23 25.69-10.23 35.19 0l104 112C320.1 126.7 321.8 136.8 318 145.6z"/></svg>
                </button>
                <button class="shuffle">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M424.1 287c-15.13-15.12-40.1-4.426-40.1 16.97V352H336L153.6 108.8C147.6 100.8 138.1 96 128 96H32C14.31 96 0 110.3 0 128s14.31 32 32 32h80l182.4 243.2C300.4 411.3 309.9 416 320 416h63.97v47.94c0 21.39 25.86 32.12 40.99 17l79.1-79.98c9.387-9.387 9.387-24.59 0-33.97L424.1 287zM336 160h47.97v48.03c0 21.39 25.87 32.09 40.1 16.97l79.1-79.98c9.387-9.391 9.385-24.59-.0013-33.97l-79.1-79.98c-15.13-15.12-40.99-4.391-40.99 17V96H320c-10.06 0-19.56 4.75-25.59 12.81L254 162.7L293.1 216L336 160zM112 352H32c-17.69 0-32 14.31-32 32s14.31 32 32 32h96c10.06 0 19.56-4.75 25.59-12.81l40.4-53.87L154 296L112 352z"/></svg>
                </button>
                <button></button>
                <button></button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512"><path d="M320 224H416c17.67 0 32-14.33 32-32s-14.33-32-32-32h-95.1c-17.67 0-32 14.33-32 32S302.3 224 320 224zM320 352H480c17.67 0 32-14.33 32-32s-14.33-32-32-32h-159.1c-17.67 0-32 14.33-32 32S302.3 352 320 352zM320 96h32c17.67 0 31.1-14.33 31.1-32s-14.33-32-31.1-32h-32c-17.67 0-32 14.33-32 32S302.3 96 320 96zM544 416h-223.1c-17.67 0-32 14.33-32 32s14.33 32 32 32H544c17.67 0 32-14.33 32-32S561.7 416 544 416zM192.4 330.7L160 366.1V64.03C160 46.33 145.7 32 128 32S96 46.33 96 64.03v302L63.6 330.7c-6.312-6.883-14.94-10.38-23.61-10.38c-7.719 0-15.47 2.781-21.61 8.414c-13.03 11.95-13.9 32.22-1.969 45.27l87.1 96.09c12.12 13.26 35.06 13.26 47.19 0l87.1-96.09c11.94-13.05 11.06-33.31-1.969-45.27C224.6 316.8 204.4 317.7 192.4 330.7z"/></svg>
                </button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><path d="M313.6 392.3l-104 112c-9.5 10.23-25.69 10.23-35.19 0l-104-112c-6.484-6.984-8.219-17.17-4.406-25.92S78.45 352 88 352H160V80C160 71.19 152.8 64 144 64H32C14.33 64 0 49.69 0 32s14.33-32 32-32h112C188.1 0 224 35.88 224 80V352h72c9.547 0 18.19 5.656 22 14.41S320.1 385.3 313.6 392.3z"/></svg>
                </button>
            </div>

            <div class="bloc_btn_grey">
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512"><path d="M31.1 64.03c-17.67 0-31.1 14.33-31.1 32v319.9c0 17.67 14.33 32 32 32C49.67 447.1 64 433.6 64 415.1V96.03C64 78.36 49.67 64.03 31.1 64.03zM267.5 71.41l-192 159.1C67.82 237.8 64 246.9 64 256c0 9.094 3.82 18.18 11.44 24.62l192 159.1c20.63 17.12 52.51 2.75 52.51-24.62v-319.9C319.1 68.66 288.1 54.28 267.5 71.41z"/></svg>
                </button>
                <button>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512"><path d="M287.1 447.1c17.67 0 31.1-14.33 31.1-32V96.03c0-17.67-14.33-32-32-32c-17.67 0-31.1 14.33-31.1 31.1v319.9C255.1 433.6 270.3 447.1 287.1 447.1zM52.51 440.6l192-159.1c7.625-6.436 11.43-15.53 11.43-24.62c0-9.094-3.809-18.18-11.43-24.62l-192-159.1C31.88 54.28 0 68.66 0 96.03v319.9C0 443.3 31.88 457.7 52.51 440.6z"/></svg>
                </button>
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
    import pokemon_list from "./assets/data/pokemon.js";

    export default {
        name: 'Pokedex',
        data() {
            return {
                pokemon: '',
                actual: 0,
            }
        },
        mounted() {
            this.getAllPokemon();
        },
        methods: {
            getAllPokemon() {
                this.pokemon = pokemon_list;
            },


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
    .select {
        cursor: pointer;
        background-color: #222222;
        box-shadow: inset 2px 2px 8px rgba(243, 243, 243, .3),
                    inset -2px -2px 8px rgba(1, 1, 1, .8);
        height: 70px;
        width: 70px;
        border-radius: 70px;
        margin: 75px 0;
    }

    .select svg {
        height: 40%;
        fill: #3e3e3e;
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
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 0 0 0 25px;
        align-self: flex-end;
        height: 150px;
        width: 150px;
    }
    .bloc_direction button  {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .bloc_direction button svg {
        height: 40%;
        fill: #3e3e3e;
    }

    .btn_dir1 {
        position: absolute;
        height: 150px;
        width: 50px;
        background-color: #222222;
        border-radius: 8px;
    }
    .btn_dir2 {
        position: absolute;
        height: 50px;
        width: 150px;
        background-color: #222222;
        border-radius: 8px;
    }
    .up {
        cursor: pointer;
        position: absolute;
        top: 0;
        border-radius: 8px;
        background-color: #252525;
        box-shadow: inset 2px 2px 4px rgba(243, 243, 243, .2);
        height: 50px;
        width: 50px;
        transform: scale(.90);
    }
    .left {
        cursor: pointer;
        position: absolute;
        left: 0;
        border-radius: 8px;
        background-color: #252525;
        box-shadow: inset 2px 2px 4px rgba(243, 243, 243, .2);
        height: 50px;
        width: 50px;
        transform: scale(.90);
    }
    .right {
        cursor: pointer;
        position: absolute;
        right: 0;
        border-radius: 8px;
        background-color: #252525;
        box-shadow: inset -2px -2px 6px rgba(1, 1, 1, .8);
        height: 50px;
        width: 50px;
        transform: scale(.90);
    }
    .down {
        cursor: pointer;
        position: absolute;
        bottom: 0;
        border-radius: 8px;
        background-color: #252525;
        box-shadow: inset -2px -2px 6px rgba(1, 1, 1, .8);
        height: 50px;
        width: 50px;
        transform: scale(.90);
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

    .bloc_btn_blue button svg {
        height: 40%;
        fill: #2277ab;
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
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        width: 65px;
        height: 65px;
        border-radius: 5px;
        box-shadow: inset 2px 2px 8px rgba(243, 243, 243, .6),
                    inset -2px -2px 8px rgba(1, 1, 1, .6);
    }
    .bloc_btn_grey button svg {
        height: 40%;
        fill: #999999;
    }

    .bloc_screen {
        margin: 65px 0 0 0;
        height: 70px;
        width: 350px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .bloc_screen div {
        height: 70px;
        width: 150px;
        background-color: #333333;
        box-shadow: inset 4px 4px 8px rgba(1, 1, 1, .5);
        border-radius: 5px;
        overflow: hidden;
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