
# Crkbd - Configuração personalizada do meu teclado split

<p align="center"><img src="https://github.com/user-attachments/assets/8ed7ae5e-146a-48ce-9c4d-cd8a6668f7bd"/></p>



Este repositório contém a configuração personalizada do firmware [ZMK](https://zmk.dev/) para o meu teclado split **Crkbd (Corne Keyboard)**.

Construí este teclado **inteiramente do zero**, desde a soldagem dos componentes até a configuração do firmware, utilizando como base o projeto open-source original:  
🔗 [foostan/crkbd](https://github.com/foostan/crkbd)

## 🛠️ Especificações do teclado

- 🔹 Layout split com 6 colunas por lado
- 🔹 3 teclas na fileira inferior lateral (polegares)
- 🔹 Switches brown
- 🔹 Keycaps brancos perfil uniforme
- 🔹 OLEDs para status e camadas
- 🔹 Firmware: [ZMK Firmware](https://zmk.dev/)

## 📁 Estrutura do repositório

```
Crkbd/
├── config/
│   ├── keymap.keymap         # Mapeamento de teclas
│   ├── shields/              # Definições específicas do hardware
│   └── ...                  
├── zmk-config/               # Configuração do ambiente ZMK
└── README.md
```

> **Nota:** O repositório pode ser adaptado para builds com QMK se necessário, mas atualmente está ajustado para ZMK.

## 🚀 Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/ImLusca/Crkbd.git
   ```

2. Siga o guia oficial do ZMK para configurar o ambiente de build:
   👉 https://zmk.dev/docs

3. Compile e flashe o firmware usando os arquivos de configuração deste repositório.

## 📸 Meu build

![photo_2025-07-04_16-46-52](https://github.com/user-attachments/assets/6ee9ff8e-bb90-44d3-8bf3-26939c76cf3a)

Teclado montado manualmente com base no projeto original. Cada peça foi soldada e montada por mim, com especial atenção à ergonomia e à portabilidade para trabalho diário e programação.

## 💡 Créditos

- Projeto original: [foostan/crkbd](https://github.com/foostan/crkbd)
- Firmware: [ZMK Firmware](https://zmk.dev/)

## 📜 Licença

Este repositório segue a licença [MIT](LICENSE).

---

Sinta-se à vontade para clonar e adaptar para seu próprio teclado split!
