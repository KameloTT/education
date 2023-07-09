# Virtualization concept

This page is described how to install, configure and use vagrant tool

Vagrant is a tool which help to install (VM)Virtual Machine(it is isolated operation system(linux or windows) in your laptop or server or public clouds. 

## Virtual Machine concept(VM)


During Virtual machine creating we have to specify how much resources will be allocated from server(or your laptop) to such VM.

Below is main resources which we define for vitrual machine

- CPU (processor cores)
- RAM (Memory, not a disk)
- DISK (disk space which will be consumed from server(or your laptop).
- Type of Operation system(Linux or Windows)
- Name (any human readable name)

VM lives on you laptop and consume your resources like any other program. Turn it off when you finish work with them or delete it to free disk capacity.

![vm][vm]

[vm]: https://www.softwarehow.com/wp-content/uploads/Virtual-Machine-2.jpg "vm"

For creation any of VMs need to use special software(program) which can control VMs and manage. 

Such type of software has name **Hypervisor**

## Hypervisor concept

Hypervior is software which can manage VM lifecycle(create, modify, delete).

There is a list most popular Hypervisors which can be installed on laptop or server

| Name | Install on Linux | Install on Windows | Production | Testing|
|------|---------------|-----------------|------------|--------|
|VirtualBox| yes | yes | no   | yes|
|Parallels | yes | no  | no   | yes|
|RHEV      | yes | no  | yes  | no
|KVM       | yes | no  | yes* | yes
|Hyper-V   | no  | yes | yes  | yes
|Vmware    | yes | no  | yes  | no


Below is diagram which shows Hypervisor role:

![hyp][hyp]

[hyp]: https://i0.wp.com/i.postimg.cc/pL0drWxX/Hypervisor-Type-II-1024x432.png?resize=583%2C246&ssl=1 "hyp"

Where:

- Hardware is server or laptop with process,memory and disk(physical device)
- OS is Operation system on server/laptop like Linux/Windows/Macos
- Hypervisor is software on our Operation system
- Guest OS is Operation system on Virtual machine which is controlled by Hypervisor on our server/laptop

### Parallels

Parallels is Hypervisor for MacOS which can be used for VM creation and management.

This is icon of such software on your laptop

<img src="https://www.wizcase.com/wp-content/uploads/2021/12/en-parallels-logo.jpg" alt="parallels" width="150" height="150"/> 

???+ warning
   
     Do not update such preinstalled Parallels on your laptop, it will be broken, 100%.

## Useful Links

* [Russian article - Vagrant]

