## Tekton and Kpack - comparison of reliable and fast path options from source repo to image repo for your Spring apps

A very typical path for getting your Spring apps from development to production involves the following steps:
Build the code, package the artifact into a container, put the container into a registry and deploy it to Kubernetes.
Many CI Tools have already adapted to the trend of containerized pipelines and being fully based on Kubernetes itself. 
Tekton and Kpack are the two examples being examined in this talk. It will provide a comparison of the two technologies with evaluation criteria 
like user friendliness, setup and configuration, robustness, operability, integration with tools and credential handling.
The majority of the evaluation will be shown in a live demo.

Adrian version:
Kubernetes has become the number one place to run your applications in the cloud. 
But its not only the applications that need to adapt to the new challenges. 
CI Systems have to come up with new solutions to not only keep up with the demand of cloud native microservices,
but also to benefit from it. 
Tekton (formely know as knative building) and kpack are two projects that aim to bring CI/CD systems on a k8s native level 
by providing the basic building blocks. 
The following talk will be an introduction to both technologies and their current status. 
Starting with a overview of the basic concepts and a quick deep dive into how they actually work under the hood. 
It will try to show how you can include kpack in your production flow and how jenkins x is using tekton already.
