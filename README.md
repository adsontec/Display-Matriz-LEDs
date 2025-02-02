## Display Matriz LEDs 🥇
Este projeto demonstra como usar o Raspberry Pi Pico W para fazer um display númerico com a matriz de LEDs (WS2812) usando dois butçoes um para incrementar e outro para decrementar o painel de LEDs, consolidando os conceitos de interrupções do microcontrolador RP2040.
## Funcionalidade: 🤠
Ao presionar o botão A incrementado o número que esta no display sendo que a numeração começa em 0 e vai até o 9, já o botão B decrementar os números. Na função principal existe um loop que faz um LED vermelho fica piscando.
## Requisitos de Hardware: ☑️
- Microcontrolador Raspberry Pi Pico W
- Matriz 5x5 de LEDs (WS2812)
- 1 LED (RGB)
- 1 Resistores de 220 Ω
- 2 Buttton (Pushbutton)
## Requisitos de Software: ☑️
- Instalar o Visual Studio Code
- Instalar a extensão Wokwi no VSCode
- Instalar os pacotes do Pico SDK
## Pinos GPIO dos LEDs 🐿️
- Matriz 5x5 (WS2812): GPIO 7
- LED (RGB): GPIO 11, GPIO 12 e GPIO 13
- Button A: GPIO 5
- Button B: GPIO6 
## Explicação do Código: 🕵️
- **stdio_init_all()**: Inicializar comunicação padrão
- **inicializar_GPIOs**: Inicializar as configurações dos pinos dos LEDs e dos putões
- **gpio_set_irq_enabled_with_callback(BUTTON_A, GPIO_IRQ_EDGE_FALL, true, &gpio_irq_handler)**: Configuração da interrupção com callback para o botão A
- **gpio_set_irq_enabled_with_callback(BUTTON_B, GPIO_IRQ_EDGE_FALL, true, &gpio_irq_handler)**: Configuração da interrupção com callback para o botão B
- **atualizar_matriz_leds(pio, sm, cont);**: Atualizar a matriz de LEDS
## Link com a produção do vídeo 📀

https://www.youtube.com/watch?v=N2EIxvV78s0

## Imagem do Projeto ✔️
![Display LED](https://github.com/user-attachments/assets/459abaf6-7636-4f81-b176-0318d061ccf1)

