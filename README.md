O seguinte repositório contém a ponderada do turtlebot teleoperado pt1.
Para realizar o que foi pedido no enunciado, o diretório contém um package chamado "turtlebot3_teleop", contendo como os pincipais scripts o teleop.py e o stop_robot_client.py.

Em teleop.py é configurado a interface de usuário e principais funcionalidades do orbô, detectando o que o usuário apertou como botão e realizando a resposta adequando com base nela. Além disso, ao apertar a barra de espaço a função de emergência é acionada como um serviço ROS, tornando o processo inutilizável ater ser reiniciado.

Já o stop_robot_client.py. configura a parte do cliente do serviço ROS e atua de forma parecida com o botão de espaço na linha de comando, tornando o robô inutilizável até ser reiniciado.

Para acionar a interface é necessário rodar no workspace o seguinte comando: `ros2 run turtlebot3_teleop teleop` . Para acionar a parada de emergência sem ser pela linha de comando, é necessário rodar `ros2 run turtlebot3_teleop stop_robot_client.` enquanto o comando anterior continua rodando em outro terminal.

O vídeo a seguir exemplifica o funcionamento da atividade: [vídeo](https://drive.google.com/file/d/1PcTrKFkN_H7jYebCHOf2il0L8SwzD8Zg/view?usp=sharing)


