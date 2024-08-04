# stock-app
#commands
#to setup minikube pv mount
ls -ld
sudo mkdir -p /mnt/data2/postgres
sudo chown -R 999:999 /mnt/data2/postgres
sudo chmod -R 755 /mnt/data2/postgres
#portforwarding
kubectl port-forward service/backend 8000:8000
kubectl port-forward service/frontend 3000:3000
#images
backend v7
frontend v14
