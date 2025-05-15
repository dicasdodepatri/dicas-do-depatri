<script setup>


</script>

<template>
    <header>
        <a href="#"><div class="logo-title"><img src="../assets/logo.svg" alt="logo" id="logo">
        <h1>DEPATRI</h1></div></a>
    </header>

    <div class="content-title">
        <h2>Consultar Dados Vazados</h2>
    </div>

    <div class="knowledge-options">
        <a href="https://haveibeenpwned.com">Meu email foi vazado?<svg width="24px" height="24px" viewBox="0 0 1048 1048" class="icon" version="1.1" xmlns="http://www.w3.org/2000/svg" fill="#434343" stroke="#434343"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M512 599.6L107.9 311.1v19.7L512 619.3l404.1-288.6V311L512 599.6z" fill="#43434334343"></path><path d="M63.9 187v650h896.2V187H63.9z m852.2 598.5L672.2 611.3l-13.8 9.8L899.1 793H125.5l240.6-171.8-13.8-9.8-244.4 174.5V231h808.2v554.5z" fill="#4343433434339393A"></path><path d="M512.9 536.7m-10 0a10 10 0 1 0 20 0 10 10 0 1 0-20 0Z" fill="#43434334343"></path></g></svg></a>
        <a href="http://cnpj.info">Abriram uma empresa em meu nome?<svg fill="#434343" width="24px" height="24px" viewBox="0 0 16.00 16.00" id="company-16px" xmlns="http://www.w3.org/2000/svg" stroke="#434343" stroke-width="0"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round" stroke="#CCCCCC" stroke-width="0.736"></g><g id="SVGRepo_iconCarrier"> <path id="Path_133" data-name="Path 133" d="M323.5-192h-9a1.5,1.5,0,0,0-1.5,1.5V-176h12v-14.5A1.5,1.5,0,0,0,323.5-192ZM318-177v-3h2v3Zm6,0h-3v-3.5a.5.5,0,0,0-.5-.5h-3a.5.5,0,0,0-.5.5v3.5h-3v-13.5a.5.5,0,0,1,.5-.5h9a.5.5,0,0,1,.5.5Zm-8-12h2v2h-2Zm4,0h2v2h-2Zm-4,4h2v2h-2Zm4,0h2v2h-2Z" transform="translate(-313 192)"></path> </g></svg></a>
        <a href="https://cadastropre.com.br">Cadastraram um telefone pré-pago em meu nome?<svg width="24px" height="24px" viewBox="0 0 24.00 24.00" xmlns="http://www.w3.org/2000/svg" fill="#434343" stroke="#434343" stroke-width="0.00024000000000000003"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round" stroke="#CCCCCC" stroke-width="1.8719999999999999"></g><g id="SVGRepo_iconCarrier"><path d="M2.725 2.24a4.385 4.385 0 0 0-1.486 4.15 22.028 22.028 0 0 0 5.833 10.537A22.028 22.028 0 0 0 17.61 22.76a3.44 3.44 0 0 0 .851.108 4.804 4.804 0 0 0 3.3-1.594 2.623 2.623 0 0 0 .914-1.686l.316-2.295a1.055 1.055 0 0 0-.766-1.162l-4.468-1.225a1.055 1.055 0 0 0-1.14.409l-1.174 1.661a.626.626 0 0 1-.733.21 15.491 15.491 0 0 1-4.546-3.35 15.491 15.491 0 0 1-3.35-4.546.626.626 0 0 1 .21-.733L8.77 7.384a1.055 1.055 0 0 0 .41-1.141L7.952 1.776A1.054 1.054 0 0 0 6.79 1.01l-2.38.316a2.623 2.623 0 0 0-1.686.914zm.78.633a1.616 1.616 0 0 1 1.074-.56L6.936 2a.056.056 0 0 1 .052.04l1.226 4.468a.093.093 0 0 1-.002.046l-1.783 1.2a1.63 1.63 0 0 0-.548 1.902 16.158 16.158 0 0 0 3.575 4.888 16.158 16.158 0 0 0 4.888 3.575 1.62 1.62 0 0 0 .595.112 1.642 1.642 0 0 0 1.32-.677l1.173-1.662a.053.053 0 0 1 .047-.022l.013.001 4.467 1.226a.055.055 0 0 1 .04.06l-.311 2.261a1.618 1.618 0 0 1-.561 1.077l-.074.073a3.907 3.907 0 0 1-2.593 1.3 2.453 2.453 0 0 1-.604-.076 21.004 21.004 0 0 1-10.08-5.575A20.996 20.996 0 0 1 2.208 6.144a3.476 3.476 0 0 1 1.224-3.197z"></path><path fill="none" d="M0 0h24v24H0z"></path></g></svg></a>
        <a href="#/ferramentas"> <svg xmlns="http://www.w3.org/2000/svg" height="32px" viewBox="0 -960 960 960" width="32px" fill="#434343"><path d="m313-440 224 224-57 56-320-320 320-320 57 56-224 224h487v80H313Z"/></svg>Voltar</a>
    </div>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.material{
    margin-left: 10px;
    margin-bottom: 10px;
}

header {
    display: flex;
    justify-content: space-between;
    padding-top: 50px;
    padding-bottom: 25px;
    align-items: center;
    width: 85vw;
    max-width: 1200px;
    margin: 0 auto;
    font-family: "FreeSans", sans-serif;
    font-weight: 800;
    letter-spacing: 2px;
}

header a {
    text-decoration: none;
    color: white;
}
.home{
    text-decoration: none;
    color: white;
    margin-top: 10vh;
    align-self: center;
    font-size: 1rem;
    text-decoration: none;
    padding: 0.75rem 1rem;
    border-radius: 10px;
    transition: background-color 0.3s ease, transform 0.3s ease;
    width: fit-content;
    transition: all 0.5s ease-in-out;

}
.home:hover{
    transform: scale(2);
}
a i {
    scale: 2;
}

header i {
    cursor: pointer;
    font-size: 2.5rem;
    padding-right: 10px;
}

.logo-title {
    display: flex;
    align-items: center;
    gap: 10px;
    cursor: pointer;
}

.knowledge-options a{
    font-size: 1.8rem;
    text-decoration: none;
    width:100%;
    color: #f2e9e4;
    padding:1rem;
    justify-content: center;
    align-items: center;
    display: flex;
    height: 80px;
    background-color: #9a8c98;
    transition: background-color 0.3s ease, transform 0.3s ease;
}
.knowledge-options{
    font-family: "TimeBurner", sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    background: rgba(200, 190, 190, 0.336);
    margin: 0 auto;
    border-radius: 10px;
    width: 0vw;
    height: min-content;
    overflow: hidden;
    text-align: center;
    animation: openScroll 1.5s forwards;
    gap: 2px;
    margin-bottom: 60px;
}
.knowledge-options a *{
    margin-left: 10px;
}
.knowledge-options  a:hover {
    background-color: #c9ada7; 
    transform: scale(1.05); 
}
#logo {
    width: 15vw;
    max-width: 120px;
    margin-right: 10px;
}
.content-title {
    font-family: "FreeSans", sans-serif;
    text-align: center;
    margin: 3rem 0;
    font-size: 3rem;
    word-spacing: 20px;
    color: #f2f2f2;
    letter-spacing: 1px;
    text-transform: uppercase;
}
@media (max-width: 768px) {
    header {
        padding-top: 30px;
        padding-bottom: 20px;
        flex-direction: column;
        align-items: center;
        text-align: center;
}
    .knowledge-options a{
        font-size: 2rem;
}

  
    .logo-title {
        flex-direction: column;
        gap: 8px;
}
    .content-title {
    font-size: 2rem;
}
  
    #logo {
        width: 20vw;
        margin-left: 0;
}
}
@media (max-width: 480px) {
    header {
        width: 95vw;
}
    .content-title {
        font-size: 1.8rem;
        margin: 2rem 0;
}
    .knowledge-options a{
        font-size: 1rem;
}

    #logo {
        width: 30vw;
        max-width: 80px;
        margin: 0;
}
}
@keyframes openScroll{
    0%{width:0vw;height:0vh;}
    100%{width:75vw;height: 280px;}
}
</style>