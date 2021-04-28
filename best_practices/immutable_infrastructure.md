Immutable/Phoenix Servers:
-------------------------
- Instances are replaced for every deployment, rather than being updated in-place.
- Practice immutable/phoenix Servers to avoid configuration drifts and ensure deployments are repeatable from source.
- Build & Package a base image thats harden, well tested and containing all depencencies and libraries.
- Provision server instances from the base image.
- Introduce change to the base image and rebuid it.
- Subject the new base image to automated regression tests.
- Replace the current instances with the instances using the latest base image.

Handling data in phoenix servers:
---------------------------------
- When implementing phoenix or immutable servers you should consider what data needs to be persisted as servers are destroyed and created, and what data must be replicated in order to scale by adding additional servers.
- Leverage Shared file system like NFS, Mountable storage volumes, Data replication techniques.

