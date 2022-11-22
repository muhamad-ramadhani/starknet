<p style="font-size:14px" align="right">
<a href="https://t.me/PemulungAirdropID" target="_blank">Join our telegram <img src="https://user-images.githubusercontent.com/72949170/194228482-0f875615-e155-4b12-8716-8111addd6cba.jpg" width="30"/></a>
</p>

<p align="center">
  <img width="60%" height="auto" src="https://user-images.githubusercontent.com/72949170/203295518-6dd98a34-856c-44cd-a629-3a4a2176a8be.png">
</p>

# STARKNET TESTNET

|  Komponen |  Persyaratan Minimum |
| ------------ | ------------ |
| CPU  | 4 core  |
| RAM | 8 GB  |
| Penyimpanan  | 100GB HDD |
| Koneksi | 100 Mbit/s |

Explorer
> https://voyager.online/

Social Media
> [ Discord ](https://discord.gg/qypnmzkhbc) | [ Twitter ](https://twitter.com/StarkWareLtd)

## 1. Register Alchemy

- [ Daftar Disini ](https://alchemy.com/?r=e8e631bf1f85c03e)

## 2. Create App

![image](https://user-images.githubusercontent.com/72949170/203296699-e2cc5a94-92e9-4f24-b149-2b333e18fb2b.png)

- Masukan detail app
- Pilih Ethereum Mainnet

![image](https://user-images.githubusercontent.com/72949170/203296934-d2781709-e73e-4ffc-99a2-de2f02204140.png)

- Masuk ke App yang sudah kalian buat
- Pilih ```View Key```
- Salin HTTPS

![image](https://user-images.githubusercontent.com/72949170/203297260-dd0ac150-fc4e-4c7e-a173-8d7147b33bd4.png)

## 3. Utiwi ke VPS & Install bahan2

jika udah ada ga perlu install lagi
- Install Docker
```
sudo apt update -y && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt install docker-ce
```
- Install bumbu kehidupan
```
sudo apt-get install -y pkg-config curl git build-essential libssl-dev screen
```

## 4. Run Node
- Install Node
```
git clone --branch v0.4.0 https://github.com/eqlabs/pathfinder.git
```
- Run Node
```
mkdir -p $HOME/pathfinder
docker run -d \
  --rm \
  -p 9545:9545 \
  --user "$(id -u):$(id -g)" \
  -e RUST_LOG=info \
  --name starknet \
  -e PATHFINDER_ETHEREUM_API_URL="HTTPSKALIAN" \
  -v $HOME/pathfinder:/usr/share/pathfinder/data \
  eqlabs/pathfinder
  ```
**Ganti ```HTTPSKALIAN``` jadi HTTPS Kalian yang tadi udah dicopy**

Contoh
> mkdir -p $HOME/pathfinder
docker run -d \
  --rm \
  -p 9545:9545 \
  --user "$(id -u):$(id -g)" \
  -e RUST_LOG=info \
  --name starknet \
  -e PATHFINDER_ETHEREUM_API_URL="https://eth-mainnet.g.alchemy.com/v2/xxxxxxxxxxxxxxxxxxxxxx" \
  -v $HOME/pathfinder:/usr/share/pathfinder/data \
  eqlabs/pathfinder
  
  ![image](https://user-images.githubusercontent.com/72949170/203298504-061dac27-34cf-4e1a-9296-440ad87a2a26.png)

## 5. Cek Log kalian
```
docker logs -f starknet
```
![image](https://user-images.githubusercontent.com/72949170/203298747-b705671a-3d92-48f0-8b75-dd5e40f0013f.png)

## 6. Cek App Alchemy kalian
Pastiin udah ada angka-angka yang nongol

![image](https://user-images.githubusercontent.com/72949170/203299119-fbce7d29-040f-48fb-9580-e93c3f6196b3.png)

- Lalu screenshot seperti screenshot diatas

## 7. Laporan ke Discord

- Post screenshot tadi ke twitter dengan tag & hashtag dibawah
```
@AlchemyLearn
@StarkNetEco

#StarkNet #starknetnode
```
- Pergi ke discord bagian ```#✅｜full-node-success```
- Kirim tweet kalian & IP VPS, kalau perlu sama screenshot yang tadi

![image](https://user-images.githubusercontent.com/72949170/203299860-52ecbe9e-cf8c-4047-95de-2b1f30f9201b.png)


## DONE, UNTUK UPDATE SELANJUTNYA KALIAN BISA PANTAU <a href="https://t.me/PemulungAirdropID" target="_blank">CHANNEL KITA </a>
