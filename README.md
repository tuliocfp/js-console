# js-console
## Red Hat Quick start Application for RHSSO 
### Running on Openshift
```bash

oc new-build --name js-console --binary --strategy source --image-stream httpd
```
```bash
oc start-build js-console --from-dir . --follow
```
```bash
oc new-app --image-stream=js-console:latest
```
```bash
```
oc expose svc/js-console
```
