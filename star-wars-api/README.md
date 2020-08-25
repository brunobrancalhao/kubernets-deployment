# star-wars-api

# Realizar o build da imagem

 ```sh
 docker build -t <usuario>/star-wars-api:tag .
 ```

# Publciar imagem no docker HUB

 ```sh
 docker push <usuario>/star-wars-api:tag
 ```

# -- Rodar o APP no cluster --

# Subir o deployment
 ```sh
 kubectl apply -f star-wars-deployment.yaml
 ```

# Subir o service
 ```sh
 kubectl apply -f star-wars-service.yaml
 ```

# Comando para expor a porta HTTPS
 ```sh
 kubectl port-forward service/star-wars-api-service 9000:9000
 ```

