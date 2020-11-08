Kubernetes - Developer Experience

Kubernetes hat sich in den letzten Jahren als die Standard Container Orchestrierung etabliert,
und ist aus der Entwicklung und insbesondere dem Betrieb von moderenen verteilten und container-basierten Anwendungen nur noch schwer wegzudenken.

Manuelle sowie automatische Skalierung von Workloads, Load Balancing, Service Discovery und dynamische Updates einer Anwendung
ohne Unterbrechung der Verfügbarkeit gehören zum kleinen einmaleins der Platform und es bietet Möglichkeiten für einfache Erweiterungen.

Es ist sowohl als lokale on-premise Lösung einsetzbar als auch bei den namhaften Cloud Providern als Managed Service leicht verfügbar.

Trotz alledem gilt: Kubernetes ist nicht einfach. Insbesondere die initiale Lernkurve ist steil.
Durch die weite Verbreitung haben sich auch die Anforderungen diesbezüglich an EntwicklerInnen verändert und vergrößert.

Wo früher das Ende der Verantwortlichkeit beim Build und Test des Codes war wird heutzutage zumindest ein Grundverständnis 
von Dingen wie Dockerfilesyntax, Pods, Ingress, ConfigMaps uvm. erhofft bzw. erwartet.

Dieser Artikel wird versuchen zu beschreiben welche zusätzlichen Kenntnisse zum Deployment und Betrieb von Anwendungen auf Kubernetes notwendig ist 
und wie diese im Vergleich zu Technologien wie Cloud Foundry, Knative und OpenShift anzusehen sind.

History Timeline?

"Plain Kubernetes"

Im folgenden Abschnitt wird dargestellt welche Schritte notwendig sind vom Quelltext Repository der Anwendung bis zur Laufzeit auf Kubernetes.
Als Beispiel zum Vergleich dient eine einfache Spring Boot Web Anwendung.

Der erste Schritt, der in jedem Fall ausgeführt werden muss ist das Erstellen eines Container Images mit der darin kompilierten bzw. lauffähigen Anwendung.
Kubernetes ist per se "Anwendungs-agnostisch", d.h. das Eintrittsticket zu der Platform ist ein Container Image. Was genau darin enthalten ist, ist aus Sicht der Platform erstmal nicht relevant.

Die traditionelle Vorgehensweise ist hier ein maven oder gradle build eines jar files, welches dann in einem Dockerfile referenziert und in ein Container Image verpackt wird.
Es gibt hier auch Alternativen z.B. maven/gradle Plugins, die diese Schritte kombinieren und automatisieren, wie z.B. der fabric8 docker maven plugin oder Spring Boot ab Version 2.3 mit Integration der Paketo Technologie.

In jedem Falle bleibt festzuhalten, daß hier Schritte notwendig sind bevor man überhaupt mit Kubernetes anfangen kann und eine Entscheidung für eine standartisierte  und konsistente Build und Container Strategie sinnvoll ist.
Sobald das Image nun gebaut ist, kann es über eine Image Registry wie. z.B. dem Docker Hub (Link) einem Kubernetes Cluster zur Verfügung gestellt werden.



