---
uid: Connector_help_Axon_ACP_GPD100
---

# Axon ACP GPD100

The GPD100 is a dual-channel 3 Gb/s, HD up-converter with color corrector and optional cross-input audio shuffler.

The **Axon ACP GPD100** connector can be used to display and configure information related to this device.

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
| 1.0.0.x   | 2522, 3128             |

### System Info

| Range     | DCF Integration     | Cassandra Compliant     | Linked Components     | Exported Components     |
|-----------|---------------------|-------------------------|-----------------------|-------------------------|
| 1.0.0.x   | Yes                 | Yes                     | -                     | -                       |

## Installation and configuration

### Creation

The element using this connector can be automatically created by the parent element using the **Axon ACP Frame Manager** connector, but it can also be a standalone element.

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
- **Status**
- **Add-On**
- **Quad Speed**
- **Video**
- **S2020**
- **Miscellaneous**
- **Dolby**
- **Encoder**
- **Loss/Detect**
- **Pro Logic**
- **MD Status**
- **Metadata**
- **DD Metadata**
- **Audio**
- **Embedder**
- **Embedder A**
- **Embedder B**
- **Embedder C**
- **Embedder D**
- **Alarm Priority**: This page displays the event messages of the card, i.e. special messages generated asynchronously on the card.

## DataMiner Connectivity Framework

The Axon ACP connector supports the usage of DCF.

DCF can also be implemented through the DataMiner DCF user interface and through DataMiner third-party connectors (for instance a manager).

### Interfaces

#### Physical Interfaces

- **SDI Input 1**: A single fixed interface of type **input**.
- **SDI Input 2**: A single fixed interface of type **input**.
- **QUAD-SPEED SYNAPSE Bus Input**: A single fixed interface of type **input**.
- **SDI Output A1**: A single fixed interface of type **output**.
- **SDI Output A2**: A single fixed interface of type **output**.
- **QUAD-SPEED SYNAPSE Bus Output**: A single fixed interface of type **output**.
