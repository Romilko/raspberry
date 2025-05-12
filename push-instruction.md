Image build and push:
 - docker build -t romilko/image:tag .
 - docker run -p [container-port]:[app-port] romilko/image:tag
 - docker push romilko/image:tag

Create secret:
 - kubectl create secret generic secret-name \
  --from-literal=KEY=VALUE \
  --from-literal=KEY=VALUE

Run pod:
  - kubectl apply -f "github raw url"
