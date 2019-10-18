---
description: >-
  Octant is an open source developer-centric web interface for Kubernetes that
  lets you inspect a Kubernetes cluster on which applications
  reside.https://github.com/vmware-tanzu/octant/projects‌
---

# Project Octant: Introduction

### Environment Overview <a id="environment-overview"></a>

‌

Your lab environment is hosted with a cloud server instance. This instance is accessible by clicking the “My Lab” icon on the left of your Strigo web page. You can access the terminal session using the built-in interface provided by Strigo or feel free to SSH directly as well \(instructions will appear in the terminal\).‌

The appropriate kubernetes related tools \(docker, kubectl, kubernetes, etc.\) have already been installed ahead of time.‌

## Prepare Your Lab <a id="prepare-your-lab"></a>

‌

### Step 1: Start Kubernetes and your Docker Registry <a id="step-1-start-kubernetes-and-your-docker-registry"></a>

```text
k8s-start
```

##  Install Octant

### ‌Step 1: Download Octant under your home directory and untar the file

```text
cd ~/ 
wget https://github.com/vmware-tanzu/octant/releases/download/v0.8.0/octant_0.8.0_Linux-64bit.tar.gz && tar -xzvf octant_0.8.0_Linux-64bit.tar.gz 
```

### Step 2 : Start Octant <a id="step-2-start-octant"></a>

```text
cd ~/octant_0.8.0_Linux-64bit/
export OCTANT_LISTENER_ADDR=0.0.0.0:7777 && ./octant
```

This will start octant on localhost at port 7777, to access the UI of Octant, click on the 'Octant' button on the top of the page within 'My Lab' 

{% hint style="info" %}
You might have to hit  'Reload this page' to see Octant UI
{% endhint %}
