🔵🟢🔴 Sequência de LEDs com Raspberry Pi Pico

Este projeto utiliza um Raspberry Pi Pico para controlar três LEDs (azul, verde e vermelho) ativados por um botão. Quando o botão é pressionado, os LEDs acendem simultaneamente e, em seguida, desligam um por um, respeitando um intervalo de 3 segundos entre cada um.

🛠️ Requisitos:

*Raspberry Pi Pico
*3 LEDs (azul, verde e vermelho)
*3 resistores (330Ω)
*1 botão push-button
Fios de conexão
Protoboard

📌 Funcionamento:

*Quando o botão é pressionado, todos os LEDs acendem ao mesmo tempo.
*Após 3 segundos, o LED vermelho apaga.
*Após mais 3 segundos, o LED verde apaga.
*Após mais 3 segundos, o LED azul apaga.
*O sistema aguarda uma nova pressão no botão para repetir o ciclo.

🔧 Configuração do Hardware

Os componentes devem ser conectados da seguinte maneira ao Raspberry Pi Pico:

Componente	GPIO
*LED Azul	11
*LED Verde	12
*LED Vermelho	13
*Botão	5
⚠️ Importante: O botão deve ser conectado com um resistor pull-up interno ativado.

🚀 Como Executar:

*Instale o SDK do Raspberry Pi Pico e configure o ambiente de desenvolvimento.
*Compile e carregue o código para o Raspberry Pi Pico.
*Pressione o botão para iniciar a sequência de LEDs.

📝 Explicação do Código:

*Configuração dos pinos: LEDs configurados como saída, botão como entrada com pull-up.
*Interrupção do botão: Ativa a sequência quando pressionado.
*Temporizadores: Controlam o tempo de desligamento de cada LED.
*Evita acionamento múltiplo: Bloqueia novas execuções enquanto a sequência estiver em andamento.
