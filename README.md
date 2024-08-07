# eth-k8s
eth k8s geth -prysm


kubectl creat -n ethereum

kubectl apply -f <deplyoment files for Geth | Prysm> 

Add bootnode to Geth example:
"--bootnodes"
          - "enode://d860a01f9722d78051619d1e2351aba3f43f943f6f00718d1b9baa4101932a1f5011f16bb2b1bb35db20d6fe28fa0bf09636d26a87d31de9ec6203eeedb1f666@18.138.108.67:30303;enode://22a8232c3abc76a16ae9d6c3b164f98775fe226f0917b0ca871128a74a8e9630b458460865bab457221f1d448dd9791d24c4e5d88786180ac185df813a68d4de@3.209.45.79:30303;enode://2b252ab6a1d0f971d9722cb839a42cb81db019ba44c08754628ab4a823487071b5695317c8ccd085219c3a03af063495b2f1da8d18218da2d6a82981b45e6ffc@65.108.70.101:30303;enode://4aeb4ab6c14b23e2c4cfdce879c04b0748a20d8e9b59e25ded2a08143e265c6c25936e74cbc8e641e3312ca288673d91f2f93f8e277de3cfa444ecdaaf982052@157"
          
 
 helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
 
 helm repo add grafana https://grafana.github.io/helm-charts

 helm install grafana grafana/grafana
 
 helm install prometheus stable/prometheus


Syncing Geth 

```
INFO [08-03|22:40:10.976] Imported new chain segment               blocks=1  txs=142  mgas=7.995  elapsed=8.229s   mgasps=0.971  number=10,291,650 hash=14c9ae…4c3621 dirty=15.96MiB
INFO [08-03|22:40:18.213] Imported new chain segment               blocks=2  txs=278  mgas=15.937 elapsed=7.237s   mgasps=2.203  number=10,291,652 hash=3fdabc…45ccfd dirty=16.02MiB
```
Syncing Prysm
```
time="2024-08-03 22:40:10" level=info msg="New gossiped block received" prefix=blockchain slot=1928374 proposerIndex=2912
time="2024-08-03 22:40:15" level=info msg="Block processed" prefix=blockchain slot=1928374 blockRoot=8e2f…3a4c stateRoot=c3d2…1f2e
```
