# aristiovaldo-o-falador (Aristiovaldo - The Talking One)
Projeto para acoplar os pequenos subsistemas que farão parte do Aristiovaldo

En-US

Aristiovaldo is an IRL (In Real Life) face with jaw motion, that will "talk" some voice records.

It will be 3 parts.

- "The Brain" - Python 
    A software that will get a written quote and turn into syllables.
    The process will be.
        - User write a quote
        - Get the google voice for that quote
        - Turn that voice clip into waves
        - Run the script to control the jaw movement based on the wave form of that voiceclip.

    The main goal is to do this in real-time like experience, so as soon as I get the wave model, the script could play the audio while controlling the Arduino
    
    I'll try to apply voice filters to original clip. If it works IT WILL BE FUCKING AWESOME.

- "The Spinal Cord" - Arduino
    A little software waiting to get commands from the brain, ready to move the "jaw muscle".
    I will be using an arduino uno R3 linked with a servo motor.

- "The Face" - The real face of the Aristiovaldo
    I tried to make an mask using a kind of paper mache, used paper and glue. 
        - Didn't look good
        - Takes forever (4 days between the start and the dried mask)
        - Maybe it isn't hard enough, so it can fall apart when I get to build the jaw mechanism.

    But if it don't work as it is, I'll buy a plastic one that I can build the thing.

    Maybe I'll put some leds. Imagine this little prick glowing while says something with a robot voice.


# O Falador
# Author: Pedro 'nPhreak' Rodrigues

"O Falador" project, a Python + Arduino project. Turn audio into jaw movement.

A ideia é criar um programinha pra transformar audio em movimentos de um servo motor.

Primeira parte é um App com python e interface capaz de pegar uma frase escrita, buscar o clipe de áudio no google e transformar em movimento para "O Rosto".

    
- O "Cérebro"
    Programa que pegará a frase e processará para fazer "O Rosto" se mover como se estivesse falando a frase. 
    O processo será mais ou menos assim:
    - Usuário digita um texto
    - O programa envia o texto para a API fo Google para receber a frase falada.
    - Analisa e transforma o áudio no formato de ondas
    - Analisa as Ondas para mexer "a boca" do Rosto 
        
- A Coluna
    Programa rodando no Arduino com conexão Serial aberta, transformando os comandos do "Cérebro" em movimentos do Servo Motor.


- A Face
    - A face é composta de uma parte "artística" e uma eletrônica

    - Artística
        - Não faço ideia se vai dar certo.
        - Fiz uma tentativa de papel machê, se der errado, eu vou comprar uma de plástico. 
    
    - Eletrônica
        - Já tenho uma ideia do mecanismo que usarei para fazer o movimento da boca, quando começar essa parte eu escrevo mais sobre.
        - Já tenho os motores, o arduino, led e tudo o mais.


Primeiro objetivo é que O Falador seja capaz de "falar" frases pela voz do Google. (Aquela do tradutor mesmo).
Dependendo da precisão da análise, tentarei utilizar filtros de voz, tornando mais divertido (assustador na verdade).