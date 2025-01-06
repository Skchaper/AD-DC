## GPO

_Le tuto suivant a été fait à partir des machines utilisées dans l'atelier GPO_

Contexte :  
* GPO fond d'écran : **User-Interface-Wallpaper-Green**  
* GPO panneau de configuration : **User-Security-ControlPanel-Deny**  
* Utilisateur utilisé sur la machine cliente : **User2**  

L'utilisateur du domaine **User2** est membre des groupes suivants :  
![VirtualBoxVM_mL4OQs5bb8.png](https://github.com/Skchaper/AD-DC/blob/main/SCREEN/SCREEN_GPO/VirtualBoxVM_mL4OQs5bb8.png)

La GPO fond d'écran s'applique aux groupes **GrpUsersWallpaper-Green** et **Ordinateurs du domaine** :
![VirtualBoxVM_f3HxvOLEV1.png](https://github.com/Skchaper/AD-DC/blob/main/SCREEN/SCREEN_GPO/VirtualBoxVM_f3HxvOLEV1.png)

Lors de la connexion de **User2** sur une machine cliente, le fond d'écran a bien été changé :
![VirtualBoxVM_2UbnXeo9Im.jpg](https://github.com/Skchaper/AD-DC/blob/main/SCREEN/SCREEN_GPO/VirtualBoxVM_2UbnXeo9Im.jpg)

La GPO panneau de configuration s'applique aux groupes **GrpUsersWindowsRestrictions** et **Ordinateurs du domaine** :
![VirtualBoxVM_IEbndo2mHz.png](https://github.com/Skchaper/AD-DC/blob/main/SCREEN/SCREEN_GPO/VirtualBoxVM_IEbndo2mHz.png)

Lorsque qu'on essaie de lancer le panneau de configuration depuis le client avec l'utilisateur **User2**, un message de restrictions apparaît :
![VirtualBoxVM_f9EXhAdGaJ.png](https://github.com/Skchaper/AD-DC/blob/main/SCREEN/SCREEN_GPO/VirtualBoxVM_f9EXhAdGaJ.png)
