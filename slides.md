## Introduction to Vagrant

John Fearnside

john@apptentive.com

[github.com/jwfearn/slides-vagrant](https://github.com/jwfearn/slides-vagrant)



## Vagrant is:
A free, open-source, command-line tool for script-based virtual machine
management.

<p class="fragment">Maintained by [Hashicorp](https://hashicorp.com/)</p>



## Advantages
<p class="fragment">Repeatable</p>
<p class="fragment">Repeatable</p>
<p class="fragment">Scriptable</p>
<p class="fragment">Common syntax</p>
<p class="fragment">Sensible defaults</p>
<p class="fragment">Shared directories</p>
<p class="fragment">Repeatable</p>



## Requires
<span class="fragment">Host OS</span>
<span class="fragment">(Mac, Windows, or Linux)</span>

<span class="fragment">Hypervisor</span>
<span class="fragment">(e.g., VirtualBox, VMware, Hyper-V, etc.)</span>



## Terminology
*Provider* - Hypervisor Adapter

*Box* - A base OS image

*Provisioner* - System for installing and configuring software within a VM



## Providers
Adapt Hypervisor-specific APIs to common Vagrant API
<ul class="fragment">
  <li>VirtualBox</li>
  <li>VMware ($)</li>
  <li>Hyper-V</li>
  <li>*others*</li>
</ul>



## Boxes
<p class="fragment">Base OS image</p>
<p class="fragment">
  Online ecosystem, [Atlas](https://atlas.hashicorp.com/), contains
  pre-built boxes, referenced by name.
</p>
<p class="fragment">One can create custom boxes</p>
<p class="fragment">Boxes often only support some Providers</p>



## Provisioners
Runs installation/configuration scripts in systems
<ul class="fragment">
  <li>shell (recommended!)</li>
  <li>Ansible</li>
  <li>Chef</li>
  <li>Docker</li>
  <li>Puppet</li>
  <li>Salt</li>
  <li>*others*</li>
</ul>



## Conventions/Defaults
<p class="fragment">`Vagrantfile`</p>
<p class="fragment">`.vagrant/` - used by Vagrant</p>
<p class="fragment">`~/.vagrant.d/` - used by Vagrant (Boxes cached here)</p>
<p class="fragment">Provisioning runs as `root`</p>
<p class="fragment">User `vagrant`</p>
<p class="fragment">Shared directory `/vagrant`</p>



## Sample Vagrantfile



## Sample provision.sh



## Common Vagrant Commands
`vagrant up`

`vagrant ssh`

`vagrant halt`

`vagrant destroy`



## Demo
