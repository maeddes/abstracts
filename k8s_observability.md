From k9s to OpenTelemetry: A guide to observability for your apps in K8s

Understanding Kubernetes can be hard. Not only in the initial learning and understanding of the concepts, but also the aspect of keeping an overview of what is happening inside at the workloads of the cluster can be challenging. How can you quickly and easily tell if your apps are healthy, well utilised and running fine?

This talk intends to look at the various aspects of Kubernetes observability and to introduce and compares multiple Open Source tools to achieve that. The range of tools covers different observability levels and requirements of different user groups.

It starts with tools simply querying the Kubernetes API and delivering the outputs in an easy-to-understand UI, goes over the possibilities of services meshes and ends with application-side logging and monitoring. For each level of observability the user has to pay a certain price in terms of configuration and runtime overhead. In turn the quality and depth of the information is different.

The intended take-away is to get a feeling which type of tooling is the right one for a given purpose. Most options will be shown in a live demonstration. Some of the technologies have a polyglot aspect and can be applied independent of the framework. This talk has a dominant focus on JVM-based applications.


KubeCon 2023

Understanding what is happening in your cluster can be challenging. How can you quickly and easily tell if your cluster and apps are healthy, well utilized and running fine?

In this tutorial, we'll look at various aspects of Kubernetes observability, and present multiple OSS solutions from the CNCF landscape and beyond to achieve that.

We will start with tools simply querying the Kubernetes API and delivering the outputs in an easy-to-understand UI (e.g. Skooner, k9s), go over sidecar-based and eBPF-based services meshes (e.g. Kiali, Hubble UI) and end with application-side logging and monitoring (e.g. OpenTelemetry, fluentd, Jaeger, Grafana). Each level of observability demands a certain price in terms of configuration and runtime overhead. In turn the quality and depth of the information is different. 

The intended take-away is to get an understanding which type of tooling is the right one for a given purpose. Most options will be shown in a live demonstration. 

Shortened (600)

Understanding what's happening in your Kubernetes cluster can be challenging. How can you quickly and easily tell if your cluster and apps are healthy, well-utilized and running fine?

We'll look at various aspects of Kubernetes observability, and view multiple open source solutions to achieve that. Each level of observability demands a price in terms of overhead with varying quality and depth of information. We'll start with tools simply querying the Kubernetes API and delivering the outputs via an easy-to-understand UI, cover sidecar and eBPF-based services meshes, logging, and tracing.



Kubernetes zu begreifen kann schwierig sein. Nicht nur beim anfänglichen Lernen und Verstehen der Konzepte, sondern auch der Überblick über das Geschehen der Workloads eines Clusters kann eine Herausforderung darstellen. Wie kann man schnell und einfach feststellen, ob die Anwendungen gesund, gut ausgelastet und reibungslos laufen?

Dieser Vortrag beabsichtigt, die verschiedenen Aspekte der "Kubernetes Observability" zu betrachten und mehrere Open-Source-Tools vorzustellen und zu vergleichen. Die Palette der Werkzeuge umfasst unterschiedliche "Flughöhen" von Observability und Anforderungen verschiedener Benutzergruppen.

Er beginnt mit Tools, die direkt die Kubernetes-API abfragen und die Ergebnisse in einer leicht verständlichen Benutzeroberfläche liefern, geht über die Möglichkeiten von Service Meshes und endet mit Logging und Überwachung auf Anwendungsebene. Für jede Beobachtbarkeitsstufe muss der Benutzer einen bestimmten Preis in Bezug auf Konfiguration und Laufzeit Overhead zahlen. Im Gegenzug ist die Qualität und Tiefe der Informationen unterschiedlich.

Das beabsichtigte Fazit ist, ein Gefühl dafür zu bekommen, welche Art von Werkzeugen für einen bestimmten Zweck geeignet ist. Die meisten Optionen werden in einer Live-Demonstration gezeigt. Einige der Technologien haben einen polyglotten Aspekt und können unabhängig vom Framework angewendet werden. Dieser Vortrag konzentriert sich hauptsächlich auf JVM-basierte Anwendungen.


old:

What is going on in my cluster?

Kubernetes can be hard. Not only in the initial learning and understanding of the concepts, but also the aspect of keeping an overview of what is happening in and around the cluster can be challenging. How can you quickly and easily tell if the cluster is healthy, well utilised and if all applications are running fine?

This talk intends to look at the various aspects of Kubernetes observability and to introduce and compares multiple Open Source tools to achieve that. The range of tools covers different observability levels and requirements of different user groups.

It starts with tools simply querying the Kubernetes API and delivering the outputs in an easy-to-understand UI, goes over the possibilities of services meshes and ends with application-side logging and monitoring. For each level of observability the user has to pay a certain price in terms of configuration and runtime overhead. In turn the quality and depth of the information is different.

The intended take-away is to get a feeling which type of tooling is the right one for a given purpose. Most options will be shown in a live demonstration.

Was geht ab in meinem Cluster?

Kubernetes kann schwierig sein. Nicht nur die initiale Lernkurve und das Verständnis der Konzepte, sondern auch der Aspekt den Überblick zu behalten was in und um den Cluster herum so passiert kann schwierig sein. Wie mann jemand schnell und einfach sehen und sagen, ob der Cluster gesund und gut ausgelastet ist sowie, daß die Anwendungen korrekt laufen?

Dieser Vortrag beabsichtige die unterschiedlichen Flughöhen der Kubernetes "observability" zu beleuchten und verschiedene Open Source Tools dafür vorzustellen und zu vergleichen.

Der Umfang geht hier von einfachen Tools, die eine vereinfachte Visualisierung der Kubernetes API bieten, deckt darüber hinaus die Möglichkeiten von sogenannten Service Meshes ab und geht bis zum anwendungsseitigem Logging und Monitoring. For jedes Level bezahlten Kubernetes Nutzer einen gewissen Preis in Punkto Konfiguration und Overhead. Im Gegenzug steigt die Detailtiefe und Qualität der dargestellten Informationen.

Gewünschtes "Take-Away" von diesem Vortrag ist ein Gefühl zu bekommen welche Kubernetes Tools die Passenden sind für den gegebenen Anlass. Die Optionen werden größtenteils in einer Live Demo gezeigt.

short:

Den Überblick über die Geschehnisse im und rund um den Kubernetes Cluster zu bewahren stellt viele vor eine gewisse Herausforderung. Dieser Talk versucht die verschiedenen Aspekte der "Observability" zu beleuchten und zugehörige Open Source Werkzeuge dafür vorzustellen. Der Umfang geht über verschiedene Flughöhen. Von "einfacher" Abfrage der Kubernetes API über Service Mesh Optionen bis hin zu Applikations-seitigem Logging und Tracing. Jedes Level erfordert einen gewissen Preis an Konfiguration und Overhead bei der Laufzeit, bietet dafür aber auch unterschiedliche Qualität der Einblicke. Der Umfang und die Optionen wird hier an verschiedenen Beispielen vermittelt.
