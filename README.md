# apicurio.repo
This is for the Forum demo.

Unfortunately everything hasn't been automated yet, so refer to artifacts/install.odt for a description on, how to install this.

```
oc new-project demo-cicd
oc new-app jenkins-ephemeral
oc new-app sonatype/nexus
oc expose svc nexus
#modify values in pipeline.yaml as it isn't automated yet
oc create -f pipeline.yaml
```
