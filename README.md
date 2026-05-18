# airpaint
Interactive blackboard 
# AirPaint Pro ⚡

Um aplicativo web minimalista de pintura aérea que utiliza Inteligência Artificial e Visão Computacional para transformar os movimentos dos seus dedos em traços neon brilhantes na tela. Tudo processado em tempo real, direto no seu navegador.

---

## ✨ Funcionalidades

*   **Pintura por Gestos:** Desenhe no ar utilizando a câmera do seu dispositivo.
*   **Rastro Neon Suavizado:** Algoritmo de interpolação linear (Filtro Passa-Baixa) que elimina tremores da webcam, proporcionando traços fluidos e curvas perfeitas.
*   **Modo Zen (Auto-Hide):** A interface de controle e o preview da câmera se ocultam automaticamente após 3.5 segundos de inatividade enquanto você desenha, garantindo imersão total.
*   **Screenshot Limpa:** Exportação inteligente em `.png` que salva exclusivamente a sua arte com fundo escuro, omitindo menus e a imagem da câmera.
*   **Privacidade Total (Edge Computing):** O processamento do modelo de IA (MediaPipe Hands) é feito 100% localmente no seu computador via WebAssembly. Nenhuma imagem ou dado de vídeo é enviado para a nuvem.

---

## 🖐️ Comandos de Gesto

O aplicativo reconhece três estados principais com base no formato da sua mão:

| Gesto | Comando | Ação |
| :--- | :--- | :--- |
| **1 Dedo Levantado** *(Indicador)* | **Desenhar** | Ativa o pincel neon na coordenada do dedo. |
| **Palma Aberta** *(Todos os dedos)* | **Apagar** | Transforma o indicador em uma borracha dinâmica. |
| **Punho Fechado** *(Dedos recolhidos)* | **Pausar** | Interrompe o traço atual sem apagar o desenho. |

---

## 🎨 Identidade Visual e UI

O design da interface foi construído seguindo uma estética moderna e profissional:
*   **Tipografia:** Poppins (Google Fonts)
*   **Paleta de Cores:** Fundo escuro absoluto, variações de cinzas metálicos para componentes estruturais e detalhes pontuais em **Rubi Neon (#c20000)**.

---

## 🚀 Como Executar o Projeto

Como o projeto foi desenvolvido em um **único arquivo HTML autocontido**, executá-lo é extremamente simples:

1. Faça o clone ou baixe este repositório.
2. Abra o arquivo `air_drawing_app.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).
3. Conceda a permissão de acesso à webcam quando solicitado.

> ⚠️ **Nota sobre Hospedagem:** Caso decida hospedar este arquivo (por exemplo, no GitHub Pages), os navegadores modernos exigem obrigatoriamente uma conexão segura **HTTPS** para liberar o acesso à câmera do usuário.

---

## 🛠️ Tecnologias Utilizadas

*   HTML5 / CSS3 (Flexbox, Grid e Backdrop Filter)
*   JavaScript Vanilla (ES6+)
*   [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) (Google)
*   HTML5 Canvas API
