<script setup>

</script>
<template>

      

  <header>
        <a href="#"><div class="logo-title"><img src="../assets/logo.svg" alt="logo" id="logo">
        <h1>DICAS DO DEPATRI</h1></div></a>
    </header>
    <div class="content-options">

    <div class="content-1">
            <img src="../assets/lock.svg" alt="lock1" class="lock">

            <h2>Conhecimento</h2>
            <span class="borda-animada"><a href="#/golpes">GOLPES MAIS COMUNS</a></span>
        </div>

        <div class="content-2">
            <img src="../assets/lock.svg" alt="lock2" class="lock">
            <h2>Ferramentas</h2>
            <span class="borda-animada"><a href="#/ferramentas">LINKS ÚTEIS</a></span>
        </div>

        <div class="content-3">
            <img src="../assets/lock.svg" alt="lock2" class="lock">

            <h2>Prevenção</h2>
            <span class="borda-animada"><a href="">DICAS IMPORTANTES</a></span>
    </div>

        <div class="content-4">
                    <img src="../assets/lock.svg" alt="lock3" class="lock">
                    <h2>Proteção on-line</h2>
                    <span class="borda-animada"><a href="">DICAS E FERRAMENTAS</a></span>
        </div>

        <div class="content-4">
                    <img src="../assets/lock.svg" alt="lock3" class="lock">
                    <h2>Atendimento</h2>
                    <span class="borda-animada"><a href="">FALE COM UM AGENTE</a></span>
        </div>

    </div>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-dark: #22223b;
    --primary-medium: #4a4e69;
    --primary-light: #f2e9e4;
    --accent: #c9ada7;
    --accent-hover: #b08d88;
    --card-shadow: 0px 4px 12px rgba(0, 0, 0, 0.4);
    --card-shadow-hover: 0px 10px 20px rgba(0, 0, 0, 0.6);
    --border-radius: 16px;
    --transition-smooth: all 0.4s cubic-bezier(0.2, 0.8, 0.2, 1);
}

body {
    background-color: #2b2b3d;
    color: var(--primary-light);
    font-family: "TimeBurner", sans-serif;
}

header {
    display: flex;
    justify-content: center;
    padding-top: 50px;
    padding-bottom: 25px;
    align-items: center;
    width: 85vw;
    max-width: 1200px;
    margin: 0 auto;
    font-family: FreeSans, Arial, sans-serif;
    font-weight: 800;
    letter-spacing: 2px;
}

header a {
    text-decoration: none;
    color: white;
    transition: opacity 0.3s ease;
}

header a:hover {
    opacity: 0.85;
}

.logo-title {
    display: flex;
    align-items: center;
    gap: 10px;
    cursor: pointer;
    transition: transform 0.3s ease;
}

.logo-title:hover {
    transform: scale(1.03);
}

#logo {
    width: 15vw;
    max-width: 120px;
    margin-right: 10px;
    filter: drop-shadow(0px 2px 4px rgba(0, 0, 0, 0.3));
}

.content-options {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 1.5rem;
    margin: 0 auto;
    padding: 2rem 0 4rem 0;
    max-width: 900px;
    width: 85vw;
}

.content-options div {
    background: linear-gradient(135deg, var(--primary-medium), var(--primary-dark));
    box-shadow: var(--card-shadow);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    padding: 2rem;
    border-radius: var(--border-radius);
    color: var(--primary-light);
    width: 280px;
    height: 350px;
    transition: var(--transition-smooth);
    position: relative;
    overflow: hidden;
}

.content-options div::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgba(74, 78, 105, 0.2), rgba(34, 34, 59, 0.2));
    opacity: 0;
    transition: opacity 0.4s ease;
    z-index: 0;
}

.content-options div:hover {
    transform: translateY(-12px) scale(1.03);
    box-shadow: var(--card-shadow-hover);
}

.content-options div:hover::before {
    opacity: 1;
}

.content-options h2 {
    font-size: 1.7rem;
    color: var(--primary-light);
    margin: 1rem 0;
    transition: color 0.3s ease-in;
    z-index: 1;
    position: relative;
}

.content-options div:hover h2 {
    color: var(--accent);
}



.borda-animada:hover {
    transform: scale(1.1);
    background-position: 112%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
}


.content-options div a {
    font-size: 0.8rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    text-decoration: none;
    color: var(--primary-dark);
    display: flex;
    align-items: center;
    width: 100%;
    height: 100%;
}



.borda-animada {
    text-align: left;  
    padding: 0.85rem 1.2rem;
    border-radius: 10px;
    width: 100%;
    background-position: 95%;
    background-size: 22px 30px;
    background-repeat: no-repeat;
    position: relative;
    color: black;
    background-color: #c9ada7; 
    transition: transform 0.3s ease, background 0.3s ease, box-shadow 0.3s ease;
    background-image: url('../assets/right-arrow-circle.svg');
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}


.borda-animada:hover::before {
    content: '';
    position: absolute; 
    top: -10px; 
    left: -10px;
    width: 35px; 
    height: 3px;
    background: linear-gradient(to right, rgba(0, 128, 0, 0.2), rgba(0, 255, 0, 0.95)); 
    z-index: -1;
    border-radius: 10px;
    animation: move-around 3.5s linear infinite;
}

@keyframes move-around {
    0% {
        top: -10px; 
        left: -10px; 
        transform: rotate(0deg);
    }
    34% {
        top: -10px; 
        left: calc(91% + 10px); 
        transform: rotate(0deg); 
    }
    35% {
        top: -10px;
        left: calc(91% + 10px);
        transform: rotate(90deg);
    }
    49% {
        top: calc(100% + 10px);
        left: calc(91% + 10px); 
        transform: rotate(90deg); 
    }
    50% {
        top: calc(91% + 10px);
        left: calc(91% + 10px);
        transform: rotate(180deg); 
    }
    84% {
        top: calc(91% + 10px);
        left: -24px; 
        transform: rotate(180deg); 
    }
    85% {
        top: calc(91% + 10px);
        left: -24px;
        transform: rotate(270deg); 
    }
    100% {
        top: -10px; 
        left: -24px; 
        transform: rotate(270deg);
    }
}


@keyframes animatedgradient {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}

.lock {
    width: 80px;
    height: auto;
    filter: drop-shadow(0px 3px 5px rgba(0, 0, 0, 0.5));
    transition: all 0.5s ease;
    z-index: 1;
}

.content-options div:hover .lock {
    transform: rotate(15deg) scale(1.1);
    filter: drop-shadow(0px 5px 8px rgba(0, 0, 0, 0.6)) brightness(1.1);
}

@media (max-width: 768px) {
    header {
        padding-top: 30px;
        padding-bottom: 20px;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }

    .logo-title {
        flex-direction: column;
        gap: 8px;
    }

    #logo {
        width: 20vw;
        margin-left: 0;
    }

    .content-options {
        max-width: 90vw;
        gap: 2rem;
        padding: 1rem 0 3rem 0;
    }

    .content-options div {
        width: 260px;
        height: 320px;
        padding: 1.5rem;
    }

    .content-options h2 {
        font-size: 1.5rem;
    }
}

@media (max-width: 480px) {
    header {
        width: 95vw;
    }

    h1 {
        font-size: 1.5rem;
    }

    #logo {
        width: 28vw;
        max-width: 80px;
        margin: 0;
    }

    .content-options {
        flex-direction: column;
        align-items: center;
        gap: 1.5rem;
        max-width: 85vw;
        padding: 0.5rem 0 2.5rem 0;
    }

    .content-options div {
        width: 100%;
        max-width: 280px;
        height: auto;
        min-height: 280px;
        padding: 1.5rem;
    }

    .content-options h2 {
        font-size: 1.3rem;
        margin: 0.7rem 0;
    }

    .borda-animada {
        padding: 0.75rem 1rem;
    }
}


</style>
