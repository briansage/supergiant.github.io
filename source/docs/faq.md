# Supergiant Frequently Asked Questions

### What is Supergiant?
Supergiant is a data center management system that is built on Kubernetes. It’s purpose is to help make managing stateful apps in a containerized environment easier and more performant.

### Why should I use Supergiant instead of Kubernetes?
We support all uses of Kubernetes, as it is an awesome platform. We wanted to make it easier to use by making stateful, distributed apps easier to manage out of the box. Of course, if you want to reach your Kubernetes cluster within Supergiant, you can.

### What is a Supergiant app?
An app performs a function for your organization. It is made of microservices called Components. You can have multiple Apps in your Supergiant cloud, and each app can have multiple Components.

### What is a Supergiant component?
Components are microservices required by your Apps. In Supergiant, you can use public or private Docker repos to create components, making it easy to use them in the distributed, stable environment of Kubernetes.

### What are Supergiant volumes?
Volumes are persistent data stores for your components.

### How is Supergiant Licensed?
Supergiant is a publicly available repo on GitHub, and has an Apache 2 license.

### Is there any cost to running Supergiant?
Nope. Supergiant is open-source and free forever, but, of course, if you provision infrastructure, you will be charged the applicable rate by your infrastructure provider.

### Why Should I use Supergiant?
Supergiant can decrease your infrastructure costs, increase networking performance, and increase stability. See following FAQ’s.

### How does Supergiant decrease costs?
First, Supergiant can dramatically optimize the CPU utilization of your AWS infrastructure. The packing algorithm can distribute compute resources where needed, giving you needed burstability without requiring additional VM’s. Second, because of the first, your infrastructure needs can be much more predictable, giving you the ability to leverage Reserved Instance and other forward contracts, which can reduce your infrastructure costs by up to 60%.

### How does Supergiant increase networking performance?
The networking bandwidth assigned to AWS’ smaller and cheaper instances can hamper performance. With Supergiant, by putting a large number of small containers on larger instances, your instances can have the networking performance of the larger instances.

### How does Supergiant increase stability?
Supergiant is developed by the Qbox DevOps team to host distributed apps at a global scale. We built it on top of Kubernetes, an automated deployment and ops platform developed by Google. Supergiant distributes resources across multiple servers to the Apps that need them, and if hardware fails, it automatically restores what is missing, making scalable, reliable deployments easy and accessible to developers.
