<p align="center">
  <img height="100" height="auto" src="https://github.com/user-attachments/assets/44916e3e-b384-4a91-8f8a-22156a66110b">
</p>

# Gensyn Testnet

Official documentation:
>- [Validator setup instructions](https://docs.gensyn.ai/)

Explorer:
>- [Explorer](https://gensyn-testnet.explorer.alchemy.com/)

### Minimum Hardware Requirements
 - 8x CPUs; the faster clock speed the better
 - 16GB RAM
 - 100GB of storage (SSD or NVME)

### Recommended Hardware Requirements 
 - 16x CPUs; the faster clock speed the better
 - 32GB RAM
 - 500GB of storage (SSD or NVME)

 - Ubuntu 22.04

Устанавливаем ноду:

```
sudo apt update & sudo apt upgrade -y
```

```
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev git-all protobuf-compiler screen -y
```

```
curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash
```

```
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl screen git yarn && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn
```

```
npm install -g npm@11.3.0
```

```
rm -rf rl-swarm && git clone https://github.com/zunxbt/rl-swarm.git && cd rl-swarm
```

```
screen -S gensyn
```

```
python3 -m venv .venv && source .venv/bin/activate && ./run_rl_swarm.sh
```

После того как у Вас появится данное сообщение переходим по ссылке которую получите в терминале. Она будет выглядить примерно так: https://farmer-may-gotten-merge.trycloudflare.com Если страница не грузится включайте VPN. Терминал не закрываем!

![NVIDIA_Overlay_3A4K3rgnvV](https://github.com/user-attachments/assets/5abd7e4c-b39b-4325-9a5f-24f3237f5890)

Нажимаем Login и вводим свою почту. Используйте ту почту которую Вы ранее не использовали для этой ноды. На почту придет код, вводим его. 

![NVIDIA_Overlay_pHpmln91yj](https://github.com/user-attachments/assets/4a053622-1c20-4475-bdfe-eb6ad1210ae7)

После успешного входа Вы получите такое сообщение. Закрываем эту страницу и переходим в терминал. Далее продолжится установка автоматически.

![NVIDIA_Overlay_Nyu3cWufct](https://github.com/user-attachments/assets/ac421e89-656b-4989-ae25-955313381484)

Вы увидете данное сообщение, пишем N - Enter.

![NVIDIA_Overlay_ffjo2B9OS6](https://github.com/user-attachments/assets/45e233df-1174-4bc6-af84-0c66513af394)

Далее сохраняем слово после Hello и peer ID. Пример как выглядит слово: opaque stalking rabbit Пример как выглядит ID: Qmd5xKv5ocbmYDYkR1zxpexQn8TfDC1UCRRtgDVwwCZhLL

![NVIDIA_Overlay_v2s2hG6p2N](https://github.com/user-attachments/assets/157203d6-c615-44e3-bb74-eafc2b44f354)

Закрыть скрин CTRL + A + D

Зайти обратно в скрин ``screen -r gensyn``

Посмотреть Dashboard можно через сутки на этом сайте (вводим кодовое слово, которое сохраняли ранее) - https://dashboard.gensyn.ai/

Так же есть другая статистика через Ваш ID - https://gensyn-node.vercel.app/
