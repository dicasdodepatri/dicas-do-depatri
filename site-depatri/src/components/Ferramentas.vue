<script setup>
</script>

<template>
    <header>
        <a href="#"><div class="logo-title"><img src="../assets/logo.svg" alt="logo" id="logo">
        <h1>DEPATRI</h1></div></a>
    </header>

    <div class="content-title">
        <h2>Links úteis</h2>
    </div>

    <div class="knowledge-options">
        <a href="https://whois.com">whois <svg class="material" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#434343"><path d="M160-160q-33 0-56.5-23.5T80-240v-480q0-33 23.5-56.5T160-800h640q33 0 56.5 23.5T880-720v480q0 33-23.5 56.5T800-160H160Zm0-80h640v-400H160v400Zm278-58L296-440l58-58 84 84 168-168 58 58-226 226Zm-278 58v-480 480Z"/></svg></a>
        <a href="https://haveibeenpwned.com">consultar dados vazados <svg class="material" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#434343"><path d="M784-120 532-372q-30 24-69 38t-83 14q-109 0-184.5-75.5T120-580q0-109 75.5-184.5T380-840q109 0 184.5 75.5T640-580q0 44-14 83t-38 69l252 252-56 56ZM380-400q75 0 127.5-52.5T560-580q0-75-52.5-127.5T380-760q-75 0-127.5 52.5T200-580q0 75 52.5 127.5T380-400Z"/></svg></a>
        <a href="https://virustotal.com">virusTotal <svg class="material" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="#434343"><path d="M480-200q66 0 113-47t47-113v-160q0-66-47-113t-113-47q-66 0-113 47t-47 113v160q0 66 47 113t113 47Zm-80-120h160v-80H400v80Zm0-160h160v-80H400v80Zm80 40Zm0 320q-65 0-120.5-32T272-240H160v-80h84q-3-20-3.5-40t-.5-40h-80v-80h80q0-20 .5-40t3.5-40h-84v-80h112q14-23 31.5-43t40.5-35l-64-66 56-56 86 86q28-9 57-9t57 9l88-86 56 56-66 66q23 15 41.5 34.5T688-640h112v80h-84q3 20 3.5 40t.5 40h80v80h-80q0 20-.5 40t-3.5 40h84v80H688q-32 56-87.5 88T480-120Z"/></svg></a>
        <a href="https://archive.org">Wayback Machine <svg class="material" xmlns="http://www.w3.org/2000/svg"  height="24px" viewBox="0 -960 960 960" width="24px" fill="#434343"><path d="M280-200v-80h284q63 0 109.5-40T720-420q0-60-46.5-100T564-560H312l104 104-56 56-200-200 200-200 56 56-104 104h252q97 0 166.5 63T800-420q0 94-69.5 157T564-200H280Z"/></svg></a>
        <a href="https://viewdns.info">viewDNS <svg class="material" xmlns="http://www.w3.org/2000/svg" height="40px" viewBox="0 -960 960 960" width="40px" fill="#434343"><path d="M291.25-718q-22.25 0-37.75 15.58T238-664.59q0 22.26 15.58 37.76 15.58 15.5 37.83 15.5 22.26 0 37.76-15.58 15.5-15.58 15.5-37.84 0-22.25-15.58-37.75T291.25-718Zm0 409.33q-22.25 0-37.75 15.58T238-255.25q0 22.25 15.58 37.75t37.83 15.5q22.26 0 37.76-15.58 15.5-15.58 15.5-37.83 0-22.26-15.58-37.76-15.58-15.5-37.84-15.5ZM156-839.33h647.33q16.34 0 26.5 10.16Q840-819 840-802.46V-530q0 17.28-10.17 28.97-10.16 11.7-26.5 11.7H156q-15.67 0-25.83-11.7Q120-512.72 120-530v-272.46q0-16.54 10.17-26.71 10.16-10.16 25.83-10.16Zm30.67 66.66V-556h586.66v-216.67H186.67Zm-30.67 342h644.67q15.66 0 27.5 12.17Q840-406.33 840-389.98v269.31q0 19-11.83 29.84Q816.33-80 800.67-80H159.33Q143-80 131.5-90.83 120-101.67 120-120.67v-269.31q0-16.35 10.17-28.52 10.16-12.17 25.83-12.17ZM186.67-364v217.33h586.66V-364H186.67Zm0-408.67V-556v-216.67Zm0 408.67v217.33V-364Z"/></svg> </a>
        <a href="#/"><svg xmlns="http://www.w3.org/2000/svg" height="32px" viewBox="0 -960 960 960" width="32px" fill="#434343"><path d="M359.33-241.33 120-480.67 359.33-720l47.34 47.33L248-514h592v66.67H248l158.67 158.66-47.34 47.34Z"/></svg> Voltar</a>
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
    margin-bottom: 6px;
    width: 28px;
    height: 28px;

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
    100%{width:75vw;height: 480px;}
}
</style>