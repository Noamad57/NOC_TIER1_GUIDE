# ArgoCD


#### Getting Started

* Get acquainted with the concept of GitOps, and the general purpose of ArgoCD. You can read [this article](https://codefresh.io/learn/gitops/) for a good explanation.

#### Basic Questions:

1. In a general sense, how does ArgoCD enable a GitOps workflow?
2. What is an ArgoCD Application?
3. What does it mean to sync an Application?
4. What are the two sync policy types for an Application?
5. What is an ArgoCD AppProject? What are some use cases for it?
6. How do you connect a git repo to your ArgoCD instance through the UI?
7. How do you make API requests to an ArgoCD instance? how do you get the authentication token?
8. What does reconcilliation mean in the context of ArgoCD?
9. What is an app of apps pattern?
10. What is an Applicationset? how is it different than an app of apps?
11. By default, how do Applications determine which resources they are managing in the cluster?
12. When deleting an Application through the UI, you can choose whether and how to delete that Application's resources. How is this reflected in the Applications yaml?
13. What does the `preserveResourcesOnDeletion` field in an ApplicationSet do?
14. What do the `resource.exclusions` and `resource.inclusions` fields in ArgoCD's configuration do?


## Final Task


#### Prerequisites

Ask your trainer to prepare for you:
- [ ] Namespace in OpenShift (from compute)
- [ ] ArgoCD instance (from k8s services)

#### Task Steps:
1. Create a new project in GitLab. In the repository you should have yaml files of the following kubernretes resources:
  - [ ] Hello-world deployment
  - [ ] Service
  - [ ] Route
2. Connect your GitLab repository to your ArgoCD instance
3. Create an application in ArgoCD that deploys the `hello-world` manifests in your OpenShift namespace. 
4. Delete the application and watch the resources in your OpenShift namespaces. What happened to the resources managed by the application?
5. Redeploy the same resources using ArgoCD. This time, create the application using an app of apps instead of manually. 
6. In your Git repo, create 2 directorys:
  - [ ] Bruno
  - [ ] Toffee
  In each directory, add a yaml file with a configMap manifest. The name of the configMap should be the same as the directory. 
7. Using an applicationset, deploy the configMaps (bruno & toffee) in your OpenShift namespace. 
