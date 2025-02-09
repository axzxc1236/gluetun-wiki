# Wireguard options

## Environment variables

If using the Wireguard protocol, depending on the provider, the following might be compulsory:

| Variable | Default | Choices | Description |
| --- | --- | --- | --- |
| `WIREGUARD_PRIVATE_KEY` | | Valid base 58 Wireguard key | Wireguard client private key to use. This is usually always needed. |
| `WIREGUARD_ADDRESSES` | | Valid IP network interface address in the format `xx.xx.xx.xx/xx` | This is usually needed. |
| `WIREGUARD_PUBLIC_KEY` | | Valid base 58 Wireguard key | Wireguard server public key to use. This may or may not be needed. |

💁 The following environment variables are all optional:

| Variable | Default | Choices | Description |
| --- | --- | --- | --- |
| `WIREGUARD_PRESHARED_KEY` | | Base64 pre-shared key | Wireguard pre-shared key |
| `WIREGUARD_IMPLEMENTATION` | `auto` | `auto`, `kernelspace` or `userspace` | Wireguard implementation to use |
| `WIREGUARD_MTU` | `1400` | Any positive value up to `65535` | Wireguard MTU |
