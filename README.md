<p align="center">
  <img src="assets/camille.png" alt="Camille, the mascot of Liko" width="240">
</p>

<h1 align="center">rabbitmq-cluster-operator.liko</h1>

**This repository contains the RabbitMQ Cluster Operator module for the Liko data language. This module is officially maintained by the Liko team.**

It contains the complete set of RabbitMQ Cluster Operator schema definitions from the official [RabbitMQ Cluster Operator repository](https://github.com/rabbitmq/cluster-operator/releases).

---

## Installation

Initialize a local module with `liko init`, then add `rabbitmq-cluster-operator.liko` as a dependency.

```bash
liko init
```
```bash
liko add rabbitmq-cluster-operator
```

```bash
liko install
```

## Usage

The module can now be used from any directory within the current module.

```liko
#Rmq: import "rabbitmq-cluster-operator/v1beta1"


$: {
    cluster: #Rmq.RabbitmqCluster {
        metadata: {
            name: "broker"
        }
        spec: {
            replicas: 3
        
    }
}
