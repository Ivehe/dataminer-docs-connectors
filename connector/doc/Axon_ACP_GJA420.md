---
uid: Connector_help_Axon_ACP_GJA420
---

# Axon ACP GJA420

The GJA420 is 3 Gb/s, HD, SD embedded domain loudness controller based on J?nger Audio algorithms.

The **Axon ACP GJA420** connector can be used to display and configure information related to this device.

## About

This connector can be automatically generated by the connector **Axon ACP Frame Manager**.

There are different possibilities available for **alarm monitoring** and **trending**.

### Version Info

| Range     | Key Features                 | Based on     | System Impact     |
|-----------|------------------------------|--------------|-------------------|
| 1.0.0.x   | Initial version [SLC Main]   | -            | -                 |

### Product Info

| Range     | Supported Firmware     |
|-----------|------------------------|
| 1.0.0.x   | 0706                   |

### System Info

| Range     | DCF Integration     | Cassandra Compliant     | Linked Components     | Exported Components     |
|-----------|---------------------|-------------------------|-----------------------|-------------------------|
| 1.0.0.x   | Yes                 | Yes                     | -                     | -                       |

## Installation and configuration

### Creation

The element using this connector can be automatically created by the parent element using the **Axon ACP** connector, but it can also be a standalone element.

### Connections

#### Serial Main Connection

This connector uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Interface connection:

  - **IP address/host**: The polling IP or URL of the destination.
  - **Bus address**: The bus address of the device, being the slot number of the card.

#### Serial Broadcast Connection

This connector uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Interface connection:

  - **IP address/host**: The polling IP or URL of the destination.
  - **Bus address**: The bus address of the device.

## Usage

The element has the following data pages:

- **General**: This page displays general information about the card: **Card Name**, **Card Description**, **SW Revision**, **HW Revision**, etc.
- **Video**
- **S2020**
- **Loudness Engine**
- **Loudness Program**
- **Embedder A**
- **Embedder B**
- **Embedder C**
- **Embedder D**
- **Embedder Addon Status**
- **SDI I/O Status**
- **Metadata**
- **Metadata Status**
- **Alarm Priority**: This page displays the event messages of the card, i.e. special messages generated asynchronously on the card.

## DataMiner Connectivity Framework

The Axon ACP connector supports the usage of DCF.

DCF can also be implemented through the DataMiner DCF user interface and through DataMiner third-party connectors (for instance a manager).

### Interfaces

#### Physical Interfaces

- **SDI Input 1**: A single fixed interface of type **input**.
- **SDI Input 2**: A single fixed interface of type **input**.
- **SDI Output 1**: A single fixed interface of type **output**.
- **SDI Output 2**: A single fixed interface of type **output**.

### Connections

#### Internal Connections

The following connections are established:

- **SDI-1**: Between **SDI Input 1** and **SDI Output 1**.
- **SDI-2**: Between **SDI Input 2** and **SDI Output 1**.
