# Tekton Github Webook
Create tekton event listener and trigger template for github webhook using `ClusterTriggerBinding`

### Steps
- Replace necessary values in eventlistener.yaml and triggertemplate.yaml
- Apply yaml files
- Create a Route for EventListener service `oc expose svc el-github-listener`
- Copy the hostname
- Go to Github > Settings > Webhook > add webhook > paste your hostname (inculde http://) to payload URL and select content type: json
