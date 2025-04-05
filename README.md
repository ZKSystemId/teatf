# **Bulk-transfer-tea By ETRx Crypto ( DWYOR !!! )**
Send bulk transfer for Tea sepolia testnet

Fitur :
- Autosend Token Kalian secara random seharian ke user yang sudah KYC di tea ( Source database ada di bagian paling bawah )
- Pengiriman token di set secara random dalam 24 jam dan akan otomatis berlanjut di hari selanjutnya
- Batas transaksi per hari 101 - 110 ( karna direkomendasikan 101 Transaksi saja perhari )
- Ada delay per transaksi agar transaksi terlihat lebih natural
- Fitur tambahan notifikasi telegram setiap transaksi berhasil

_**YOK DIMULAI**_

# Claim Faucet kalian
Claim disini : https://faucet-assam.tea.xyz/#/


# Deploy Token
Deploy Disini : https://sepolia.tea.xyz/address/0x847d23084C474E7a0010Da5Fa869b40b321C8D7b?tab=write_contract

**Notes : Sesudah deploy, copy contract address token kalian**

# Clone repositorynya
```
git clone https://github.com/ZKSystemId/teatf.git
cd teatf
```

# Create screen ( Biar bisa running di background )
```
screen -Rd bulktransfer
```

# Install NPM , dotenv sama axios dulu di Linux
```
apt install npm
```
```
npm install dotenv
```
```
npm install axios
```

# Install Dependencies

```
npm install ethers
```

Step by Step menggunakan botnya :
- Pastikan kalian sudah menyelesaikan semua hal diatas
- Buka file .env di editor text vps kalian
- Cari bagian PRIVATE_KEY_KALIAN dan isi dengan private key kalian
- Cari bagian CONTRACT_ADDRESS dan paste contract address token kalian
- Cari bagian RPC_URL dan CHAIN_ID , pastikan sesuai dengan RPC dan Chain ID terbaru Tea Sepolia

> ( Opsional ) kalo kalian pengen dapetin notifikasi dari bot telegram, silahkan ikuti step berikut ( kalau tidak minat silahkan di skip dan langsung save saja file .envnya )
- Bot Tokennya silahkan kalian buat botnya dan ambil bot tokennya disini : https://t.me/BotFather
- Telegram Chat ID silahkan ambil disini : https://t.me/Check_Telegram_IDBot
- Copy dua duanya dan paste dibagian Bot Token dan Telegram Chat ID
- Save file .env nya
- Jalankan scriptnya pake command ini :
```
  node teatransfer.js
```
- Masukkan jumlah penerima dan Jumlah token yang akan dikirim
- Selesai, selamat berbulking bulking ria~

Notes :
- Kalo kalian pengen botnya jalan di background, pencet CTRL A + D .
- Kalo kalian mau balikin lagi botnya , pakai command ini
```
screen -r bulktransfer
```
- Kalo kalian mau matiin, tinggal klik CTRL + C

Join our telegram community here : https://t.me/ETRxCrypto

Thanks for the Source :
- KYC Adresses : https://tea.daov.xyz/kyc-address
- Original Script : https://github.com/ashev33/bulk-transfer-tea
- GPT
