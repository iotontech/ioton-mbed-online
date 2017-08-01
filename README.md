PLATAFORMA TON COM O MBED ONLINE COMPILER
=======================

A seguir os pocedimentos para usar a Placa TON com o compilador online do mbed.

## **O que é necessário previamente:**
1. Clique neste [link](https://developer.mbed.org/platforms/Seeed-Arch-Max/add/) para criar uma conta no *mbed compliler* e adicionar a *platform - Seeed Arch Max* (possui o mesmo microcontrolador da Placa TON).
2. O UPLOAD para a placa tem que ser manual, para isto é necessário baixar e descompactar este [repositório](https://github.com/iotontech/ioton-mbed-online/archive/master.zip).
3. Em algumas versões do **Windows** o driver instalado automaticamente não compatível. Para instalar o driver correto, favor realizar os seguintes passos:
    * Baixar o software Zadig: http://zadig.akeo.ie/
    * Colocar a Placa TON em modo UPLOAD (pressionando o botão *RESET/BOOT* por mais de 1s)
    * Abrir o Zadig e selecionar: *Options > List All Devices*
    * Selecionar *STM32 Bootloader* ou *WinUSB*
    * Clicar em *“replace driver”* ou *“install driver”*


## **Passo a passo de utilização:**
1. Importar algum dos códigos de exemplo a seguir:
    * [Projeto em branco](https://developer.mbed.org/compiler/#import:/teams/IOTON-Technology/code/ton_template/)
    * [Código de demonstração](https://developer.mbed.org/compiler/#import:/teams/IOTON-Technology/code/ton_demo/)
    * [Código de testes do TON-BOT](https://developer.mbed.org/compiler/#import:/teams/IOTON-Technology/code/ton-bot_teste/)
2. Faça suas edições. Aproveite o controle de versão, clicando em *Commit*. E volte versões facilmente clicando em *Revision*
3. Compilar o código ao clicar em *Compile*, será realizado o download de um arquivo *.bin*
4. Salvar ou mover este arquivo para dentro da pasta *ioton-mbed-online-master*
5. Procedimentos para gravação do código:
    * Colocar o TON no modo **BOOT**: pressionar o botão *RESET/BOOT* por mais de 1s
    * Realizar o **upload**: executar o programa *upload_ton_linux* ou *upload_ton_windows*
    * Aguardar o término do processo
    * Voltar o TON para a execução: pressione rapidamente o botão *RESET/BOOT*
