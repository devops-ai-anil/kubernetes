## Kubernetes Architecture

```mermaid
graph TD
    User --> LoadBalancer
    LoadBalancer --> Ingress
    Ingress --> Service
    Service --> Pod
    
---

# 🔵 STEP 3: View Diagram

👉 Where it works automatically:

- GitHub README ✅  
- GitLab ✅  
- VS Code (with Mermaid extension)  

---

# 🟡 STEP 4: Use Online Editor (Optional)

👉 Go to:
https://mermaid.live

- Paste code
- See diagram instantly
- Export as PNG/SVG

---

# 🔥 REAL DEVOPS EXAMPLE (FOR YOUR PROJECT)

Use this 👇

```mermaid
graph TD
    User --> LoadBalancer
    LoadBalancer --> Ingress
    Ingress --> Service
    Service --> Pod

    Pod --> Logs
    Logs --> ClaudeAI

    ClaudeAI --> Analysis
    Analysis --> AutoHealing

    AutoHealing --> Kubernetes

    Prometheus --> Pod
    Grafana --> Prometheus

    GitHubActions --> Deployment
    Deployment --> Kubernetes
