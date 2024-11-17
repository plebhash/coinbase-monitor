# Sv2 Template Coinbase Monitor

`coinbase-monitor` is a Rust application that monitors the Coinbase Transaction under the **Template Distribution** subprotocol of **Stratum V2** (Sv2 TDP).

The [`demand-easy-sv2`](https://github.com/demand-open-source/demand-easy-sv2) crate is used as the main dependency.

The executable connects to a Sv2 Template Provider (Sv2 TP) to monitor new block templates for Sv2 mining.

## UI

The executable can be customized via std env variables.

- `SERVER`: points to Sv2 TP, defaults to `127.0.0.1:8442`
- `COINBASE_OUT_DATA_SIZE`: informs Sv2 TP about expected coinbase data size limit, defaults to `34`

## Usage

### Prerequisites

- Rust (edition 2021)
- Sv2 Template Provider server compatible with Stratum V2 Template Distribution subprotocol