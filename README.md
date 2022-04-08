# ContainerInsightsLog

This tool will collect:
* linux ds and rs pods;
* windows pod;
* deployment logs.

How to run:
```
wget https://raw.githubusercontent.com/MSNina123456/ContainerInsightsLog/main/AKSInsightsLogCollection.sh && bash ./AKSInsightsLogCollection.sh
```

Output:
```
Preparing for log collection...
Prerequistes check is done, all good
Collecting logs from omsagent-5kwzn...
Complete log collection from omsagent-5kwzn!
Collecting logs from omsagent-win-25zdt, windows pod will take few minutes for log collection, please dont exit forcely...
Complete log collection from omsagent-win-25zdt!
Collecting logs from omsagent-rs-6fc95c45cf-qjsdb...
Complete log collection from omsagent-rs-6fc95c45cf-qjsdb!
Collecting onboard logs...
configMap named container-azm-ms-agentconfig is not found, if you created configMap for omsagent, please use command to save your custom configMap of omsagent: kubectl get configmaps <configMap name> --namespace=kube-system -o yaml > configMap.yaml
Complete onboard log collection!

Archiving logs...
log files have been written to azure-monitor-logs.tgz in current folder
```
