# instalar microk8

1) seguir las instruciones de https://microk8s.io/#get-started

2) para agregar dashboard kubernetes

https://microk8s.io/docs/addon-dashboard

con eso, ya es posible acceder desde el localhost, sin embargo sei se accede desde fuera, ejemplo que esto este corriendo en una maquina virtual hay que ahcer un paso mas.

```bash
microk8s kubectl port-forward -n kube-system service/kubernetes-dashboard --address <ip maquina virtual> 10443:443
```


