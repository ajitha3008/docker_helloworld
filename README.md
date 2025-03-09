# docker_helloworld
# Pre-requisites
- VS code Editor
- Node CLI & npm using “brew install node”
Verify using “node -v” & “npm -v”
- Install postman and login
- ngrok - brew install ngrok & Add auth token ngrok. 
Auth token is received after signing up
- Install Docker Desktop and login and 
then go to Settings ->Kubernetes -> Turn on “Enable Kubernetes”
Cluster choose anything from the both.
Apply and restart

# init
npm init
npm install express

# Dockerize
Docker init
docker compose up —build

To run in Background: 
docker compose up --build -d
docker compose down

https://docs.docker.com/guides/nodejs/containerize/

# Kubernetes

Create kubernetes yaml file (config file)
kubectl apply -f docker-node-kubernetes.yaml

Check:
 kubectl get deployments
 kubectl get services

kubectl delete -f docker-node-kubernetes.yaml

# Tutorial steps

- Create web app , run in localhost
- Dockerize container(using docker compose)
Optional: database , test cases
- Upload to GitHub
- Connect GitHub and docker using access tokens, variables and secrets
- Create workflow & check its running
- Turn on kubernetes
- Create kubernetes yaml file
- Orchestrate using the kubernetes(kubectl command)
Enjoy!!!





