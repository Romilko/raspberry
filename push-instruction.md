Image build and push:
 - docker build -t romilko/image:tag .
 - docker run -p [container-port]:[app-port] romilko/image:tag
 - docker push romilko/image:tag

Run pod:
  - kubectl apply -f "github raw url"
