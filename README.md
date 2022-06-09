Docker best practices

- Include installers in your project
- Have a canonical build system that builds everything completely from scratch
- Tag your builds with the git hash of the code that built it
- Use small base images such as alpine
- Build images you share publicly from Dockerfiles, always
- Dont ever leave passwords hidden in the layers of dockerfile

Kernels - what they do
- Responds to messages from the hardware
- Start and schedule programs
- Control and organize storage
- Pass messages between programs
- Allocates resources, memory, CPU, network, and so on
- AND DOCKER MANAGES KERNELS
- - uses cgroups to contain processes
- - uses namespaces to contain network
- - uses copy-onwrite filesystems to build images
