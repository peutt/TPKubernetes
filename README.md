# TPKubernetes
2a\. On crée un cluster Kubernetes à l'aide de Kind : `kind create cluster`
![Screenshot](ScreenShots/q2a1.png)
Ensuite On crée un fichier deploiement.yaml pour le pod Nginx et on lance le deploiement du pod : `kubectl apply -f deploiement.yaml`
![Screenshot](ScreenShots/q2a2.png)
On peux vérifier que le pod Nginx est en cours d'exécution avec la commande suivante : `kubectl get pods`
![Screenshot](ScreenShots/q2a3.png)
----------------------------------------------------
2b\. grace à la commande precédente nous avons obtenu le nom du pod. Avec celui-ci, on peux accéder à la page par défaut de notre pod Nginx grace à cette command : `kubectl port-forward nginx-pod 8080:80`
![Screenshot](ScreenShots/q2b1.png)
Ainsi, la page d'acceuil Nginx est accessible sur http://localhost:8080
![Screenshot](ScreenShots/q2b2.png)
