<script setup>
// Importações podem ser adicionadas aqui se necessário
</script>

<template>
  <div class="not-found-container">
    <header>
      <a href="#"><div class="logo-title"><img src="../assets/logo.svg" alt="logo" id="logo">
      <h1>DICAS DO DEPATRI</h1></div></a>
    </header>
    
    <div class="error-content">
      <div class="error-card">
        <img src="../assets/lock.svg" alt="lock" class="lock">
        <h2>Página não encontrada</h2>
        <p>Desculpe, mas a página que você está procurando não existe.</p>
        <span class="borda-animada"><a href="#">VOLTAR PARA HOME</a></span>
      </div>
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

.not-found-container {
    min-height: 100vh;
    background-color: transparent;
    color: var(--primary-light);
    font-family: "TimeBurner", sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
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

.error-content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-grow: 1;
    padding: 2rem 0;
    width: 85vw;
    max-width: 900px;
}

.error-card {
    background: linear-gradient(135deg, var(--primary-medium), var(--primary-dark));
    box-shadow: var(--card-shadow);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1.5rem;
    padding: 3rem;
    border-radius: var(--border-radius);
    color: var(--primary-light);
    width: 100%;
    max-width: 500px;
    transition: var(--transition-smooth);
    text-align: center;
}

.error-card:hover {
    transform: translateY(-8px);
    box-shadow: var(--card-shadow-hover);
}

.error-card h2 {
    font-size: 2rem;
    color: var(--primary-light);
}

.error-card p {
    font-size: 1.2rem;
    line-height: 1.6;
    margin-bottom: 1rem;
}

.lock {
    width: 100px;
    height: auto;
    filter: drop-shadow(0px 3px 5px rgba(0, 0, 0, 0.5));
    transition: all 0.5s ease;
}

.error-card:hover .lock {
    transform: rotate(15deg) scale(1.1);
    filter: drop-shadow(0px 5px 8px rgba(0, 0, 0, 0.6)) brightness(1.1);
}



.borda-animada a {
    font-size: 1.3rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;
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

    .error-card {
        padding: 2rem;
    }

    .error-card h2 {
        font-size: 1.7rem;
    }

    .error-card p {
        font-size: 1rem;
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

    .error-content {
        width: 95vw;
        padding: 1rem 0;
    }

    .error-card {
        padding: 1.5rem;
    }

    .error-card h2 {
        font-size: 1.5rem;
    }
    
    .error-card p {
        font-size: 0.9rem;
    }

    .borda-animada {
        padding: 0.75rem 1rem;
        width: 90%;
    }
}
</style>