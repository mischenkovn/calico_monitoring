#Enable monitoring
Get monitoring for prometheus-operator from calico addons

In kubespray enable monitoring for calico:
``` 
calico_felix_prometheusmetricsenabled=true 
```

#Add monitoring

replace ips 172.17.0... to your real nodes ips.

```
kubectl apply -f monitoring_calico.yaml
```

#Grafana

Grafana dashboard is 11092 