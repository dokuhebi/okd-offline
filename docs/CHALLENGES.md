# Challenges

## Air Gapped

OKD, as with most docker/container based applications, assume access to the internet, at least for initial configuration.  While OKD can [act as a registry for containers](https://docs.openshift.com/container-platform/4.1/registry/architecture-component-imageregistry.html), the docker-based version of OKD assumes it has internet connectivity to pull down the OKD and Kubernetes containers.  

## Transfer Size

While the easiest method for transfer of an operational OKD system to an air-gapped network would be to export and transfer a virtual machine, the size of an entire virtual machine may be prohibitive to actually transfer.  This may be a moot point if the containers being transferred are significantly larger than the underlying software.

## Transferrability

The solution needs to be usable across any platform supported by OKD.  This may not happen initially, but will be a goal.

## Ease of Use

OKD (and Kubernetes in general) is a very complex system with many optional components.  Our goal is to simplify the concept to minimize the learning curve.  This may mean that certain features aren't implemented or that we only support a rigid configuration.