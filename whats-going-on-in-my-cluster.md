What is going on in my cluster?

Kubernetes can be hard. Not only in the initial learning and understanding of the concepts, but also the aspect of keeping an overview of what is happening in and aroud the cluster can be challenging.
How can you quickly and easily tell if the cluster is healthy, well utilised and if all applications are running fine?

This talk intends to look at the various aspects of Kubernetes observability and to introduce and compares multiple Open Source tools to achieve that.
The range of tools covers different observability levels and requirements of different user groups.

It starts with tools simply querying the Kubernetes API and delivering the outputs in an easy-to-understand UI, goes over the possibilities of services meshes and ends with application-side logging and monitoring.
For each level of observability the user has to pay a certain price in terms of configuration and runtime overhead. In turn the quality and depth of the information is different.

The intended take-away is to get a feeling which type of tooling is the right one for a given purpose.
The options will be mostly demonstrated in a live demonstration.
![image](https://user-images.githubusercontent.com/11751587/111759122-91113880-889d-11eb-9166-7349f0cc32b2.png)
