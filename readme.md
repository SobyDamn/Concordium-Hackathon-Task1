
# Concordium Hackathon- Task 1

## Payout Info

0x1938b58567a139F62953fF6aBADc2dA67319640a

CCD Mannet - 

## Installing RUST and Cargo
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
![image](img/rust-install.png)

### Installing WASM

```
rustup target add wasm32-unknown-unknown
```

### Installing cargo-concordium
```
wget -O $HOME/.cargo/bin/cargo-concordium https://distribution.concordium.software/tools/linux/cargo-concordium_2.7.0
```
> Give executable permission to the file
```
chmod 755 $HOME/.cargo/bin/cargo-concordium
```
> Check if the installation is successful
```
cargo concordium --help
```

![image](img/wasm-cargo-concordium.png)

### Installing Concordium Client
```
wget -O $HOME/.cargo/bin/concordium-client https://distribution.concordium.software/tools/linux/concordium-client_5.0.2-0
```

> Give executable permission to the file
```
chmod 755 $HOME/.cargo/bin/concordium-client
```
![image](img/client-installation.png)

> Check if the installation is successful
```
concordium-client --help
```
![image](img/client-install.png)


### Web Wallet Installation
[Extention here](https://chrome.google.com/webstore/detail/concordium-wallet/mnnkpffndmickbiakofclnpoiajlegmg?hl=en-US)

![image](img/wallet-ext1.png)

### Claiming 2000 CCD
![image](img/ccd-claim.png)

### Exporting Private Key
![image](img/export-key.png)

### Export Account from Web Wallet
```
concordium-client config account import 32SMQBHUrLDxP6uex4RuQfPHsG98AF3XTLFJxeP4H8Ep2Fg7QN.export --name my-wallet
```
![image](img/export.png)