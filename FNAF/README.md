# 🎮 Five Nights at HTML's

**Five Nights at HTML's** é uma recriação **100% web (HTML, CSS e JavaScript puro)** do clássico *Five Nights at Freddy’s (2014)*, focada em fidelidade de mecânicas, tensão psicológica e gerenciamento de recursos, tudo rodando diretamente no navegador, sem engines externas.

---

## 📌 Visão Geral

Você assume o papel do **vigia noturno** da Freddy Fazbear’s Pizza e precisa sobreviver das **12 AM às 6 AM**, controlando portas, luzes e câmeras, enquanto quatro animatrônicos tentam chegar até você.

O jogo simula:
- IA probabilística baseada em nível
- Consumo dinâmico de energia
- Progressão de noites
- Custom Night totalmente configurável
- Sistema de salvamento via `localStorage`

---

## 🕹️ Modos de Jogo

### ▶️ Novo Jogo
- Progressão normal da **Noite 1 até a Noite 5**
- A dificuldade aumenta automaticamente a cada noite
- Desbloqueia novos modos conforme o progresso

### 🌙 6ª Noite
- Noite bônus com **IA extremamente agressiva**
- Todos os animatrônicos em níveis altos fixos

### ⚙️ Custom Night
- Desbloqueada após concluir a Noite 6
- Permite configurar individualmente o nível de IA de:
  - Freddy
  - Bonnie
  - Chica
  - Foxy
- Cada animatrônico pode variar de **0 a 20**

---

## 🔋 Sistema de Energia

A bateria começa em **100%** e diminui constantemente ao longo da noite.

### Consumo base:
- Passagem do tempo (consumo contínuo)

### Consumo adicional:
- Porta esquerda fechada
- Porta direita fechada
- Monitor de câmeras aberto

⚠️ **Se a energia chegar a 0%**, Freddy ataca automaticamente.

---

## 🎥 Sistema de Câmeras

- Abertura manual do monitor
- Mapa interativo com múltiplas salas
- Efeito de estática dinâmico
- Indicador REC piscante
- Visualização dos animatrônicos por ícones

### Pirate Cove (CAM 1C)
- Área exclusiva do Foxy
- Possui um painel especial de status
- Pode ser “resetado” ao observar diretamente

---

## 🤖 Animatrônicos & Mecânicas de IA

Cada animatrônico possui **comportamento único**, controlado por níveis de IA e decisões probabilísticas.

---

### 🐰 Bonnie (Esquerda)

- Ataca exclusivamente pela **porta esquerda**
- Estados possíveis:
  - `START` → Palco
  - `DOOR` → Porta
- Move-se com base em chance aleatória (`Math.random`)
- Se chegar à porta e ela estiver aberta:
  - O jogador tem um **tempo de reação**
  - Caso não feche a porta → **jumpscare**

📌 **Contra-medida:**  
Fechar a porta esquerda ou usar a luz para confirmar a presença.

---

### 🐔 Chica (Direita)

- Ataca exclusivamente pela **porta direita**
- Funcionamento semelhante ao Bonnie
- Estados:
  - `START`
  - `DOOR`
- Tempo de reação depende da média do nível de IA

📌 **Contra-medida:**  
Fechar a porta direita e usar a luz para confirmação visual.

---

### 🐻 Freddy Fazbear

- Animatrônico mais estratégico do jogo
- **Não aparece nas portas através das luzes**
- Movimenta-se apenas pelas câmeras
- Caminho fixo de movimentação: 1A → 1B → 7 → 6 → 4A → 4B → PORTA

#### Regras especiais:
- Só ataca se:
  - Estiver na porta
  - A porta direita estiver aberta
  - O monitor estiver **fechado**
- Pode ser afastado ao ser observado na câmera onde está.

📌 **Contra-medida:**  
Monitoramento constante das câmeras e controle rigoroso da porta direita.

---

### 🦊 Foxy

- Funciona por **estágios**, não por salas
- Estados de agressividade:
  - `0` → Dormindo
  - `1` → Espiando
  - `2` → Pronto
  - `3` → Saindo
  - `4` → Correndo

- Avança automaticamente se:
  - Não estiver sendo observado
  - O jogador não estiver na Pirate Cove

#### Ataque:
- Ao atingir o estágio 4:
  - Se a porta esquerda estiver fechada:
    - Foxy recua
    - Drena energia adicional
  - Se estiver aberta:
    - **Jumpscare imediato**

📌 **Contra-medida:**  
Verificar frequentemente a Pirate Cove e manter controle da porta esquerda.

---

## ⏱️ Relógio & Progressão

- Cada hora dura aproximadamente **45 segundos**
- O turno vai de **12 AM até 6 AM**
- Sobreviver até 6 AM conclui a noite

---

## 💾 Sistema de Salvamento

- Progresso salvo automaticamente no navegador
- Utiliza `localStorage`
- Desbloqueia:
  - Continuar jogo
  - 6ª Noite
  - Custom Night

---

## 🔊 Sistema de Áudio

Todo o áudio é gerado em tempo real usando **Web Audio API**, incluindo:
- Estática das câmeras
- Portas abrindo e fechando
- Luzes
- Corrida do Foxy
- Sons de jumpscare

Nenhum arquivo de áudio externo é utilizado.

---

## 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript Vanilla
- Web Audio API
- LocalStorage API

---

## ⚠️ Aviso Legal

Este projeto é uma **fan game não-oficial**.  
Todos os direitos dos personagens pertencem a **Scott Cawthon**.

---

## 👤 Autor

Projeto desenvolvido como um **protótipo de engine FNAF em web**, focado em:
- Lógica de IA
- Sistemas de jogo
- Atmosfera e tensão

---

Boa noite… e boa sorte. 🕯️