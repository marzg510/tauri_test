# tauri_test


- [WSL2でtauriを動かすときにやったこと](https://zenn.dev/yubachiri/scraps/caeb5d1f4c740e)

- [Tauri公式](https://tauri.app/)

```bash
sh <(curl https://create.tauri.app/sh)
```


- [Prerequistes](https://tauri.app/v1/guides/getting-started/prerequisites/)

- install
```bash
sudo apt update
sudo apt install libwebkit2gtk-4.0-dev \
    build-essential \
    curl \
    wget \
    libssl-dev \
    libgtk-3-dev \
    libayatana-appindicator3-dev \
    librsvg2-dev
curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
source ~/.cargo/env 
rustc --version
cargo install tauri-cli
```
- create app
```bash
sh <(curl https://create.tauri.app/sh)
cd tauri-app
cargo tauri dev
```


## Create Kanban App

- [軽量RustフレームワークTauriでデスクトップアプリ開発をはじめよう](https://gihyo.jp/article/2022/10/rust-monthly-topics-02)

```bash
rustc -V
node -v
yarn -v
cargo-tauri -V

yarn create tauri-app
>kanban
>yarn
>react-ts

cd kanban
yarn
yarn tauri dev
```


```bash
yarn add @asseinfo/react-kanban
```


```bash
cd src-tauri
cargo add dunce
cargo add sqlx
cargo add futures
cargo add directories
```

## Create Installer

```
yarn tauri build
```

## Cross Platform

https://tauri-app.translate.goog/v1/guides/building/cross-platform/?_x_tr_sl=en&_x_tr_tl=ja&_x_tr_hl=ja&_x_tr_pto=wapp