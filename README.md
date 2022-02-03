# Deployer une application

1. Ecrivez un manifest pod.yml pour déployer avec l'image mmumshad/simple-webapp-color en précisant que la color souhaitée est en rouge
voir fichier : 
##### pod.yml

2. Lancez votre pod et verifiez qu'il est bien en cours d'éxecution
#### lancer l'image : 
                   kubectl apply -f pod.yml
#### Vérifiez l'execution  :
                   kubectl get po
  
3. Exposez votre pod en utilisant la commande : kubectl port-forward <nom_du_pod> : 8080:8080 --address 0.0.0.0
 #
                kubectl port-forward <nom_du_pod> : 8080:8080 --address 0.0.0.0

4. Verifiez que l'application est bien joignable en ouvrant le port 8080 de votre node
#
                lancer dans l'url  @ip:8080
                
5. Ecrivez une manifest nginx-deployment.yml pour déployez 2 réplicas d'un pod nginx (version 1.18.0)


