-----

# Projeto de Videoconferência com WebRTC e Firebase

Este projeto é uma demonstração simples de uma videoconferência ponto a ponto (P2P) usando **WebRTC** para áudio/vídeo e **Firebase Firestore** para a sinalização (troca de informações de conexão).

-----

## Como Funciona

1.  **Inicie sua Câmera**: Clique no botão para permitir acesso à sua webcam e microfone.
2.  **Crie uma Chamada**: Clique em "Criar Chamada" para gerar um ID único. Este ID é o "convite" para a sua chamada.
3.  **Entre na Chamada**: Em outro dispositivo ou aba do navegador, insira o ID gerado e clique em "Atender".
4.  **Conexão P2P**: Após a troca de informações via Firebase, a conexão P2P WebRTC é estabelecida, e você verá e ouvirá o outro participante.

-----

## Configuração Necessária

1.  **Clone o Repositório**:
    ```bash
    git clone https://github.com/Nandobez/WebRTC-test-for-a-project.git
    cd WebRTC-test-for-a-project
    ```
2.  **Instale as Dependências**:
    ```bash
    npm install
    ```
3.  **Configure o Firebase**:
      * Crie um projeto no [Console do Firebase](https://console.firebase.google.com/).
      * Adicione um aplicativo web ao seu projeto.
      * Copie suas credenciais `firebaseConfig` e cole-as no arquivo `main.js`, substituindo os valores `your data`.
      * Habilite o **Firestore Database** no seu projeto Firebase.

-----

## Como Executar

1.  **Inicie o Servidor de Desenvolvimento**:
    ```bash
    npm run dev
    ```
    Este comando iniciará um servidor local e abrirá a aplicação no seu navegador (geralmente em `http://localhost:5173` ou uma porta similar).
2.  **Uso Rápido**:
      * Abra duas abas/janelas com a aplicação.
      * Em ambas, clique **"Iniciar Câmera"**.
      * Em uma aba, clique **"Criar Chamada (oferta)"** e copie o ID gerado.
      * Na outra aba, cole o ID e clique **"Atender"**.

Pronto\! Sua chamada P2P deverá estar ativa.

-----
