
Virtual machines, or VMs, provide an abstraction layer for CPU, memory, and storage

that can be changed without having to invest in new hardware,
while still allowing the environment to be flexible and secure.

With VMs, you're in control.
You decide the operating system, install tools and packages.
And your app runs either in isolation or with the other apps you install into the VM.
But there are downsides. VMs can only run one operating system at a time.
So if you have multiple server apps that all require different runtime environments,
they may also require multiple virtual machines to execute properly.
And because the VM is emulating a full computer,
tasks like starting one up or taking a snapshot are pretty slow, often taking several minutes.
But there's a lighter-weight solution that solves some of these issues. Containers.
A container bundles a single app and its dependencies,
referred to as containerizing the app, then deploys it as a unit to a container host.
The container host provides a standardized runtime environment,
which abstracts away the operating system and infrastructure requirements,
allowing the containerized application to run side-by-side with other containerized apps.

An easy way to differentiate between VMs and containers is
virtual machines virtualize the hardware,
while containers virtualize the operating system.

The operating system level virtualization of containers is one reason
why the container approach is more efficient than a full virtual machine.
It allows you to run multiple lightweight containers on a single host
without sacrificing the isolation that the virtual machine originally offered.
Azure supports several container variations, the most popular being Docker.
Unlike VMs, you can spin up containers quickly.
You're just waiting for the app to launch instead of both the operating system and the app.
Also, containerized apps tend to be much smaller in size.
And the development process is simplified, because your
development runtime environment can look exactly like the production environment.
Another advantage to containers is that they
can be orchestrated with container cluster orchestration.
You can easily deploy and manage multiple containerized applications
without worrying about which server will host each container.
The decision of whether to use a VM or a container depends on how much flexibility you need.
If you need to completely control the environment, then you might choose a VM.
If not then the portability, performance characteristics, and management capabilities of containers might be the better choice.