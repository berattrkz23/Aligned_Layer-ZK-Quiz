# Aligned Layer ZK Quiz 

![image](https://github.com/molla202/AlignedLayer/assets/91562185/cb9fca1a-a370-4aee-b41d-546d27c4523b)



</h1>


 * [Topluluk kanalımız](https://t.me/corenodechat)<br>
 * [Topluluk Twitter](https://twitter.com/corenodeHQ)<br>
 * [Aligned Layer Website](https://alignedlayer.com/)<br>
 * [Blockchain Explorer](https://explorer.corenodehq.com/Alignedlayer-Testnet)<br>
 * [Discord](https://discord.gg/zHsXryD7)<br>
 * [Twitter](https://twitter.com/alignedlayer)<br>

### 🚧Rust Kurulumu
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

(1'i seçip enter)
```

### 🚧Foundry Kurulumu
```
curl -L https://foundry.paradigm.xyz | bash
source ~/.bashrc
foundryup
cast --version
```

### 🚧OpenSSL ve pkg-config kurulumu
```
sudo apt update && sudo apt install pkg-config libssl-dev
```

### 🚧İstediğiniz adresi import edin (tercihen burner adres) İçinde Holesky Eth bulunduğundan emin olun.
```
[ -d ~/.aligned_keystore ] && rm -rf ~/.aligned_keystore && echo "Deleted existing directory ~/.aligned_keystore." ; mkdir -p ~/.aligned_keystore && cast wallet import ~/.aligned_keystore/keystore0 --interactive
```

### 🚧Aligned Layer Reposunu çekmek için
```
[ -d aligned_layer ] && rm -rf aligned_layer && echo "Deleted existing aligned_layer directory." ; git clone https://github.com/yetanotherco/aligned_layer.git && cd aligned_layer/examples/zkquiz
```

### 🚧Son komut
```
make answer_quiz KEYSTORE_PATH=~/.aligned_keystore/keystore0
```

Bu aşamada sizlere bazı sorular soracak soruların cevabı şu şekilde: C, C, A
