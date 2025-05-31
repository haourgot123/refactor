In this tutorial, you will manage your HPP app by Helm.

## How-to Guide



```shell
cd ocr_chart
helm upgrade --install hpp .
```


# Fix quyền Jenkins

```shell
3. Run Kubectl command

kubectl create namespace jenkins
kubectl create sa jenkins -n jenkins
kubectl create token jenkins -n jenkins --duration=8760h
kubectl create rolebinding jenkins-admin-binding --clusterrole=admin --serviceaccount=jenkins:jenkins --namespace=jenkins
kubectl config view
watch kubectl get pods -n jenkins


From Jenkins
4. Configure Manage Jenkins
5. Test Connection
6. Create Sample job
7. Verify test connection
```