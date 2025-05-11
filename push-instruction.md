Image build and push:
 - docker build -t romilko/image:tag .
 - docker push romilko/image:tag
 - docker run -p [host-port]:[container-port] image-name

Run pod:
  - kubectl apply -f "github raw url"
