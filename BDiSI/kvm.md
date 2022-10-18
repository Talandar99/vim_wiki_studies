# Kernel Virtual Machine

## What is KVM?
- KVM (for Kernel-based Virtual Machine) is a full virtualization solution for Linux on x86 hardware containing virtualization extensions (Intel VT or AMD-V). 
- It consists of a loadable kernel module, kvm.ko, that provides the core virtualization infrastructure and a processor specific module, kvm-intel.ko or kvm-amd.ko.

## Why KVM is better than other virtualisation methods ?
#### Performance: 
- KVM is a type 1 or “bare metal” hypervisor, meaning it runs directly on the host machine’s physical hardware. This means it doesn’t have to load an underlying OS and has direct access to the underlying hardware without having to contend for virtualization with other software such as other operating systems and device drivers. This gives KVM an inherent advantage in terms of performance and efficiency.
#### Maturity: 
- KVM is more than 15 years old and has more than 1,000 code contributors. This high level of maturity means it’s well developed and very debugged. There are plenty of experts to go to for support and questions.
#### Scalability: 
- The KVM hypervisor automatically scales to respond to heavy loads once the number of VMs increases. It also enables clustering for thousands of nodes, which helps set the foundation for a cloud-based infrastructure.
#### Security: 
- As part of the Linux kernel source code, KVM benefits from rigorous development and testing processes, as well as continuous security patching.
#### Affordability: 
- Since it’s open source and available as a Linux kernel module, KVM costs nothing out of the box.

## links
- [KVM main page](https://www.linux-kvm.org/page/Main_Page)
- [KVM vs VirtualBox](https://blog.purestorage.com/purely-informational/kvm-vs-virtualbox-which-one-should-you-use/)
