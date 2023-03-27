server:
    connection --> mdp=prl_robot  (clavier anglais)
    connection a wifi_1 (wifi qu'on veut)
    ifconfig ----> pour prendre l'ip du server wlan0
    mushr_noetic
    export ROS_HOSTNAME=localhost
    roslaunch mushr_base teleop.launch

client:
    connection a wifi_1
    ssh robot_1@<votre ip>
    entrer le pwd = prl_robot
    docker ps (pour prend l'ID du container)
    docker exec -it <your id> bash


