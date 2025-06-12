<script setup>

</script>

<template>
  <div class="chat-container">
    <header>
      <a href="#"><div class="logo-title"><img src="../assets/logo.svg" alt="logo" id="logo">
      <h1>DICAS DO DEPATRI</h1></div></a>
    </header>
    
    <div class="chat-content">
      <div class="chat-card">
        <div class="chat-messages">
          <div class="bot-message">
            <p>Olá, sou um agente autônomo! Posso verificar se algo é golpe com base na sua história. Conta o que aconteceu que eu te ajudo! <br/>
Exemplo: Recebi uma mensagem no WhatsApp de alguém se passando por um banco pedindo meus dados pessoais [pode dar mais detalhes].</p>
          </div>
        </div>
        <div class="chat-input">
          <textarea v-model="userMessage" placeholder="Digite sua história aqui..."></textarea>
          <div class="chat-buttons">
            <span class="borda-animada"><a href="#" @click.prevent="sendMessage">ENVIAR</a></span>
            <span class="borda-animada"><a href="#">VOLTAR PARA HOME</a></span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userMessage: '',
    };
  },
  methods: {
    sendMessage() {


        const userMessage = document.querySelector('textarea').value
        axios({
        
            method: 'post',
        
            url: 'https://flask2-g3g9.onrender.com',
        
            data: {
        
                value
        
            }
        
        })
        
            .then(response => console.log(response))
        
            .catch(error => console.log(error));
      console.log('Mensagem enviada:', this.userMessage);
      userMessage = ''; // Limpa o campo após envio
    },
  },
};
</script>

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

.chat-container {
    min-height: 100vh;
    background-color: transparent;
    color: var(--primary-light);
    font-family: "TimeBurner", sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
}.bot-message{
    font-family:Arial, Helvetica, sans-serif;
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

.chat-content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-grow: 1;
    padding: 2rem 0;
    width: 85vw;
    max-width: 900px;
}

.chat-card {
    background: linear-gradient(135deg, var(--primary-medium), var(--primary-dark));
    box-shadow: var(--card-shadow);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    gap: 1.5rem;
    padding: 2rem;
    border-radius: var(--border-radius);
    color: var(--primary-light);
    width: 100%;
    max-width: 600px;
    transition: var(--transition-smooth);
    text-align: center;
}

.chat-card:hover {
    transform: translateY(-8px);
    box-shadow: var(--card-shadow-hover);
}

.chat-messages {
    width: 100%;
    max-height: 400px;
    overflow-y: auto;
    padding: 1rem;
    border-radius: 8px;
    background: rgba(0, 0, 0, 0.1);
}

.bot-message {
    background: var(--primary-dark);
    padding: 1rem;
    border-radius: 8px;
    margin-bottom: 1rem;
    text-align: left;
}

.bot-message p {
    font-size: 1.1rem;
    line-height: 1.6;
}

.chat-input {
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.chat-input textarea {
    width: 100%;
    min-height: 100px;
    padding: 1rem;
    border-radius: 8px;
    border: none;
    background: rgba(255, 255, 255);
    color: var(--primary-light);
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1rem;
    resize: vertical;
    outline: none;
    color: black;
    transition: var(--transition-smooth);
}

.chat-input textarea:focus {
    box-shadow: 0 0 8px rgba(255, 255, 255, 0.2);
}

.chat-buttons {
    display: flex;
    justify-content: space-between;
    gap: 1rem;
}

.borda-animada {
    background: var(--accent);
    padding: 0.8rem 1.5rem;
    border-radius: 8px;
    cursor: pointer;
    transition: var(--transition-smooth);
    flex: 1;
    text-align: center;
}

.borda-animada a {
    font-size: 1.1rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    color: var(--primary-light);
    text-decoration: none;
    display: block;
}

.borda-animada:hover {
    background: var(--accent-hover);
    transform: scale(1.05);
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

    .chat-card {
        padding: 1.5rem;
    }

    .bot-message p {
        font-size: 1rem;
    }

    .chat-input textarea {
        font-size: 0.9rem;
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

    .chat-content {
        width: 95vw;
        padding: 1rem 0;
    }

    .chat-card {
        padding: 1rem;
    }

    .chat-buttons {
        flex-direction: column;
        gap: 0.5rem;
    }

    .borda-animada {
        padding: 0.75rem 1rem;
    }
}
</style>