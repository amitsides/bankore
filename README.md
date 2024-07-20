# Bankore Infrastructure technicals OCI OKE + OCIR + 


## CI 
1. Cobol Dockerfile
2. Java EE Dockerfile
3. Github Action yaml
4. Jenkins + OCIR https://medium.com/oracledevs/how-to-using-jenkins-to-build-container-image-and-push-to-ocir-c475f46b2a8d

https://github.com/oracle-quickstart/oke-soa

# CD

Oracle Tuxedo 

https://www.oracle.com/middleware/technologies/tuxedo.html

Oracle Tuxedo Deployment on Kubernetes 

https://github.com/oracle/helm-charts/tree/main/tuxedo

Oracle Tuxedo Service Architecture Leveraging Tuxedo (SALT) bankapp Sample Application

https://github.com/oracle/helm-charts/tree/main/tuxedo/charts/tuxedo-bankapp


Oracle Charts https://github.com/oracle/helm-charts

Java Advanced Management Console (AMC) Helm Chart

https://github.com/oracle/helm-charts/tree/main/java-amc


Containerized Advanced Management Console Deployment Guide

https://docs.oracle.com/en/java/java-components/advanced-management-console/2.20/deploy-guide/containerized-advanced-management-console.html#GUID-92FF39B4-93C6-4DE3-B2C9-A57339530882

https://oracle.github.io/helm-charts/java-amc/

https://github.com/IBM/charts/tree/master/stable/ibm-websphere-liberty

https://github.com/IBM/cloud-pak/blob/master/spec/security/psp/README.md




### Ingress Controllers on Oracle Container Engine (OKE) + traefik

https://doc.traefik.io/traefik/getting-started/install-traefik/
https://medium.com/oracledevs/experimenting-with-ingress-controllers-on-oracle-container-engine-oke-part-2-96063927d2e6

    helm repo add traefik https://traefik.github.io/charts
    helm repo update
    helm install traefik traefik/traefik
    kubectl port-forward $(kubectl get pods --selector "app.kubernetes.io/name=traefik" --output=name) 9000:9000
