
## 📦 App Versions
- v1: nginx:1.19
- v2: nginx:1.21

## 📋 Steps Performed

1. **Provisioned EC2 instance**
 
2. **Installed K3s**
 
3. ![k3s nodes](https://github.com/user-attachments/assets/51821faf-5fcf-4522-b9b9-f9fabf005548)

4. **Installed Istio and enabled sidecar injection**
  
5. ![istro installed](https://github.com/user-attachments/assets/26348af7-5385-4b42-9295-c11d0a7aa9b9)

6. **Deployed app v1 and v2**
  
7. ![apply v1 v2](https://github.com/user-attachments/assets/3003a467-0ae9-498b-9600-51c954ad5ebc)

11. **Created Kubernetes Service**
12. 
13. **Configured Istio Gateway**
14. 
15. **Created DestinationRule and VirtualService**
16. 
17. **Split traffic (80% v1, 20% v2)**
18. **Verified rollout with curl and browser**

## 🔗 Accessing the App
The app was accessed via the EC2 public IP and NodePort exposed by Istio ingressgateway.

```bash
curl http://<ec2-public-ip>:<node-port>
```

![curl](https://github.com/user-attachments/assets/ce16c390-1621-4900-9fbb-30b0437459f7)
