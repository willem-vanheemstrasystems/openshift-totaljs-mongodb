This directory contains a Jenkinsfile which can be used to build
openshift-totaljs-mongodb using an OpenShift build pipeline.

To do this, run:

```bash
# create the nodejs example as usual
oc new-app https://github.com/willem-vanheemstrasystems/openshift-totaljs-mongodb

# now create the pipeline build controller from the openshift/pipeline
# subdirectory
oc new-app https://github.com/willem-vanheemstrasystems/openshift-totaljs-mongodb \
  --context-dir=openshift/pipeline --name openshift-totaljs-mongodb-pipeline
```
