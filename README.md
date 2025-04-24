
## 📦 App Versions
- v1: nginx:1.19
- v2: nginx:1.21

## 📋 Steps Performed

1. **Provisioned EC2 instance**
2. **Installed K3s**
3. **Installed Istio and enabled sidecar injection**
4. **Deployed app v1 and v2**
5. **Created Kubernetes Service**
6. **Configured Istio Gateway**
7. **Created DestinationRule and VirtualService**
8. **Split traffic (80% v1, 20% v2)**
9. **Verified rollout with curl and browser**

## 🔗 Accessing the App
The app was accessed via the EC2 public IP and NodePort exposed by Istio ingressgateway.

```bash
curl http://<ec2-public-ip>:<node-port>
