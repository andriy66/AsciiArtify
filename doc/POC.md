# Install the Argo CD
`k3d cluster create argo`

`kubectl create namespace argocd`

`kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml`
# Running the Argo on localhost with ports 8080
`kubectl port-forward svc/argocd-server -n argocd 8080:443`

# Get the password for the admin user
Input the username - **admin**

`kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo`

# Login with the admin user data
username: admin
password: generated using the script above