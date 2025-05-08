# ROS2_trabalho
Repositório do trabalho de Robótica Probabilística 
README

O projeto desenvolvido pelos alunos Carlos Vinicius Ximenes Matos Diederichs, Jean Raposo Soares de Jesus e Igor Pinheiro Torres, sob orientação da professora Milena Faria Pinto, consiste na criação de um ambiente de simulação robótica utilizando o ROS2 (Robot Operating System 2) integrado ao simulador Gazebo.

Foi criado um workspace chamado project_ws, contendo o pacote Fla, que reúne os arquivos do robô, incluindo sua descrição em formato SDF, scripts de movimentação, sensores e o ambiente simulado. O robô foi modelado com sensores como IMU, rodas com juntas do tipo revolute e sistema de colisão. O mundo simulado inclui oito paredes com geometrias distintas, servindo como obstáculos.

A movimentação do robô é realizada pelas setas do computador, controlada via teclado através do pacote teleop_twist_keyboard, que envia comandos pelo tópico /cmd_vel. A estrutura do projeto é organizada com os arquivos launch.py, CMakeLists.txt e package.xml, que integram o ROS2 ao Gazebo, configuram os nós de simulação e definem as dependências do pacote.

O arquivo launch.py automatiza o lançamento da simulação, conecta o ROS2 ao Gazebo e ativa sensores como a IMU. Já o CMakeLists.txt compila o projeto e gerencia as bibliotecas necessárias, enquanto o package.xml descreve o pacote e suas dependências.
