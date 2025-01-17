---
id: configuration-file
title: "Configuration File"
description: The description of fields in config.toml file
author: kashish
---

:::info
Please provide correct relative/absolute path in KeystorePath and PasswordPath fields in the configuration file. The KeystorePath field should have file with `.key` extension.
:::

### Variable Description

The `config.toml` file in the repository contains various fields that should be configured in order to run various [CLI](https://github.com/Lagrange-Labs/client-cli) commands.

- `EthereumRPCURL`: Ethereum mainnet RPC endpoint for mainnet, and Holesky RPC endpoint for testnet.

- `L1RPCEndpoint`: Ethereum mainnet RPC endpoint for both mainnet and Holesky testnet.

- `BeaconURL`: Beacon mainnet RPC endpoint for both mainnet and Holesky testnet.

- `L2RPCEndpoint`: Rollup (Optimism or Base) chain's mainnet RPC endpoint for both mainnet and Holesky testnet.

- `BLSCurve`: Currently, we only support `BN254` curve.

- `ConcurrentFetchers`: This parameter can be used to control the number of parallel fetchers that are responsible to fetch a block. Default value is `8`.

- `OperatorKeystorePath` = EigenLayer operator keystore file path

- `OperatorKeystorePasswordPath` = EigenLayer operator keystore password file path

- `SignerECDSAKeystorePath` = ECDSA singner keystore file path

- `SignerECDSAKeystorePasswordPath` = ECDSA signer keystore password file path

- `BLSKeystorePath` = BLS keystore file path

- `BLSKeystorePasswordPath` = BLS keystore password file path

- `MetricsServiceName` = The service name used for the metrics. Default is `lagrange-node`.

- `PrometheusRetentionTime` = Rentention time for Prometheus metrics data. Default is `60s`.
