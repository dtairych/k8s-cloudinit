# Cloud Init for K8s

This repo holds a public cloud init file to bring a Debian 12 server into a compliant state to run Kubernetes.  This cloud init is primarily used by *BK8soX* in conjunction with Equinix Metal to build bare Metal Kubernetes environments on demand. 


The focus for this "compliance" is on:
- Installing the appropriate packages
- Setting up firewall / security to restrict communication at the host level
  - Allowing SSH
  - Kubernetes control ports
  - Calico networking
  - Portworx storage
 
For any other service, be it for Kubernetes, or publishing an external service, additional ports might need to be permitted on the firewalls.   
