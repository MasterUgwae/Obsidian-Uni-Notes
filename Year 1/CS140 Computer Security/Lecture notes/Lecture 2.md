# 

## Types of vitualisation
- Bare-metal virtualisation
	- Above the hardware is a hypervisore
		- the multiplle OS run on the hypervisore
	- One Domain is called Domain0
		- All other OSs have to call Domain0 to access the hardware
- QEMU
	- Hypervisor runs above the host operating system
	- Hardware are simulated as files.

## QEMU Commands

```bash
qemu-img
qemu-kvm -m 
```

## Basic terminology

- Asset 
	- Anything you want to protect
- Vulnerablility
	- A flaw or weakneess in a system that could be exploited.
- Threat
	- A potential for violation of security.
	- It is when an attecker has both capability and intention
- attack
	- An assult on security in which a threat actor exploits vulnerability to realise the threat
- Risk
	- An expectation of loss 