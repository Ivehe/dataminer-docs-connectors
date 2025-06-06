---
uid: Connector_help_Axon_ACP_GXG100
---

# Axon ACP GXG100

The **GXG100** card is low-latency up-, down-, and cross-converter with 16-channel audio transparency.

The Axon ACP GXG100 connector is used to monitor and configure the GXG100 card.

## About

### Version Info

| Range                | Key Features     | Based on     | System Impact     |
|----------------------|------------------|--------------|-------------------|
| 1.0.0.x [SLC Main]   | Initial version  | -            | -                 |

### Product Info

| Range     | Supported Firmware     |
|-----------|------------------------|
| 1.0.0.x   | 6583                   |

### System Info

| Range     | DCF Integration     | Cassandra Compliant     | Linked Components     | Exported Components     |
|-----------|---------------------|-------------------------|-----------------------|-------------------------|
| 1.0.0.x   | Yes                 | Yes                     | -                     | -                       |

## Configuration

### Connections

#### Serial Main Connection

This connector uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Interface connection:

  - **IP address/host**: The polling IP or URL of the destination.
  - **IP port**: The IP port of the destination (fixed value: *2071*).
  - **Bus address**: The bus address or slot number/position of the card in the frame.

#### Serial IP Connection - Events Connection

This connector uses a smart-serial connection and requires the following input during element creation:

SMART-SERIAL CONNECTION:

- Interface connection:

  - **IP address/host**: The polling IP or URL of the destination. Specify "any".
  - **IP port**: The IP port of the destination (fixed value: *2071*).
  - **Bus address**: The bus address or slot number/position of the card in the frame.

## How to use

The setting of some parameters depends on other parameters' current value. For example, on the Network page, in order to set the Preferred IP Address, you need to make sure the IP Configuration is set to *Manual* mode. You first set the required parameter to the appropriate value before you set the other parameter.

## DataMiner Connectivity Framework

The **1.0.0.x** connector range of the Axon ACP GXG100 connector supports the usage of DCF.

DCF can also be implemented through the DataMiner DCF user interface and through DataMiner third-party connectors (for instance a manager).

### Interfaces

#### Fixed interfaces

Physical fixed interfaces:

- **SDI Input 1**: A single fixed interface of type **in**.
- **SDI Input 2**: A single fixed interface of type **in**.
- **SDI Output A1**: A single fixed interface of type **out**.
- **SDI Output A2**: A single fixed interface of type **out**.
- **SDI Output B1**: A single fixed interface of type **out**.
- **SDI Output B2**: A single fixed interface of type **out**.

### Connections

#### Internal Connections

- **SDI Input 1 -\> SDI Output A1**.
- **SDI Input 1 -\> SDI Output A2**.
- **SDI Input 1 -\> SDI Output B1**.
- **SDI Input 1 -\> SDI Output B2**.
- **SDI Input 2 -\> SDI Output A1**.
- **SDI Input 2 -\> SDI Output A2**.
- **SDI Input 2 -\> SDI Output B1**.
- **SDI Input 2 -\> SDI Output B2**.
