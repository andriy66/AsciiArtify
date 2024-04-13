# The comparison table of minikube, k3s and kind

| Feature            | Minikube                                   | K3S                                     | Kind                                 |
|--------------------|--------------------------------------------|-----------------------------------------|--------------------------------------|
| Deployment Ease    | Relatively complex setup and configuration | Simple setup and configuration          | Simple setup and configuration       |
| Resource Usage     | High resource usage due to running VM      | Low resource usage                      | Moderate resource usage              |
| Speed              | Slower due to VM overhead                  | Faster due to lightweight components    | Moderate speed, faster than Minikube |
| Cluster Size       | Suitable for small to medium clusters      | Suitable for small to medium clusters   | Suitable for testing, small clusters |
| Docker Integration | Uses Docker to run Kubernetes              | Uses containerd as the default runtime  | Uses Docker to run Kubernetes        |
| Production Ready   | Not recommended for production use         | Suitable for lightweight production use | Not recommended for production use   |
| Features           | Full Kubernetes features                   | Subset of Kubernetes features           | Limited features, focused on testing |
| Community Support  | Large community support                    | Growing community support               | Growing community support            |
| Use Cases          | Local development and testing              | Lightweight deployments, edge computing | Local development and testing        |
| Documentation      | Extensive documentation available          | Good documentation available            | Good documentation available         |

# Minikube

![minikube.gif](..%2Fresources%2Fminikube.gif)

# K3S

![k3s.gif](..%2Fresources%2Fk3s.gif)

# Kind

![kind.gif](..%2Fresources%2Fkind.gif)

# Conclusion
**Kind** is good for local development and testing of Kubernetes applications. Using for creating lightweight, self-contained Kubernetes clusters using Docker containers.

**K3S** is for lightweight Kubernetes deployments in resource-constrained environments. Using for edge computing, IoT, development environments, testing, and production deployments.

**Minikube**  is for local development and testing of Kubernetes applications with a focus on compatibility with cloud environments. Using for developing and testing applications locally before deploying them to a production Kubernetes cluster.

**For conclusion** our team chosen the **Kind**, because it meets the project requirements.