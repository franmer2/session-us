Il se peut que dans le cadre d’un déploiement de Microsoft Purview ou Microsoft Fabric, vous ayez besoin de gérer la session des utilisateurs en forçant la déconnection automatique après un certain laps de temps d’inactivité. Dans cet article, je vais expliquer commencer paramétrer la déconnexion automatique pour ces 2 solutions.

# Microsoft Purview

1.	Avec un compte Global Admin, connectez-vous au portail Azure (https://portal.azure.com).
2.	Cliquez sur l’engrenage en haut à droite de l’écran.
3.	Cliquez sur « **Signing out + notifications** ».
4.	Dans la rubrique « **Signing out** », cochez la case « **Enable directory level idle timeout** » puis définissez le délai avant la fermeture de session.

![image](Images/001.png)


Ci-dessous une fin de session de Microsoft Purview :

![image](Images/010.png)



# Microsoft Fabric

1.	Connectez-vous avec un compte global admin sur le site du centre d'administration d'office 365. (https://admin.microsoft.com/)
2.	Dans les menus à gauche de l’écran, cliquez sur « **Settings** », puis sur « **Org settings** ». ![image](Images/002.png)


3.	En haut de l’écran, cliquez sur l’onglet « **Security & privacy** », puis sur « **Idle session timeout** ».![image](Images/003.png)


4.	Dans le panneau qui s’affiche alors sur la droite, cochez la case « **Turn on to set the period of inactivity to users to be signed off of Microsoft 365 web apps** ». Puis définissez le délai avant la fin de session.![image](Images/004.png)

5. **Attention !!** Le paramètre peut prendre plusieurs heures pour s'appliquer à l'ensemble de vos utilisateurs 

Ci-dessous une fin de session de Microsoft Fabric :

![image](Images/011.png)