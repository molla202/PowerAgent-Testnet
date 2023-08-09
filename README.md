![Addddddddddsız](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/06eb3f43-4ca6-406d-9b4e-7e9e62a2cd9a)


 
 * [Topluluk kanalımız](https://t.me/corenodechat)<br>
 * [Topluluk Twitter](https://twitter.com/corenodeHQ)<br>



## Sistem Gereksinimleri
| Bileşenler | Minimum Gereksinimler | 
| ------------ | ------------ |
| CPU |	4 |
| RAM	| 8 GB |
| Storage	| 200 GB SSD |


### Not: Dikkat ediniz.
 - cosmos harici çalışan bir proje varsa yuksek ihtimalle portlarda sorun çıkar.
## Kütüphane ve gerekli yazılımları kuralım.
sudo wget -O - https://prerequisites.dappnode.io | sudo bash
## Oto Kurulum Script
sudo wget -O - https://installer.dappnode.io | sudo bash
## Profil oluşturuyoruz.
source /usr/src/dappnode/DNCORE/.dappnode_profile
## Çalışanma durumunu kontrol edelim.
dappnode_status
## vpn için bilgilerini alalım.
dappnode_wireguard
not: çıkan çıktıyı bir metin belgesine kaydedin.
## vpn bağlantısı için kendi bilgisayarımıza programı indirelim.
Windows
https://download.wireguard.com/windows-client/wireguard-installer.exe

MacOS
https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1&mt=12
not: kurun ve açın.
![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/4c5f8f74-bd94-4a21-aab5-d365b8e674a8)
- daha sonra açılan ekranın ortasında yazanları sil seçip ve yukarıda dappnode_wireguard yazdığımızda çıkan kaydettiğimiz çıktıyı bu yerin içine kaydedelim ve en başındakine isim verelim.
![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/198c19f4-8a27-4b82-8a7b-5fc58504dbb2)
- programın ortasında etkinleştir yazıyor. tıklayın etkinleşmesini bekleyin.
## Daha sonra internet tarayıcınızı açın ve bu adresine gidin
http://my.dappnode/#/
- buna benzer bir adres gelecek kullanıcı adı ve şifre yazma yerleri olucak. burda giriş için kullanıcı olusturuyoruz. 
* kullanıcı adı yaz
* şifre yaz
* tekrar şifre yaz
not: şifre sayılar ve bir buyuk harf olması gerekiyor. onaylamadan sonra bilgilerinizi kaydedin ve giriş yapın. sonunda bir key çıkacak bunuda kaydediniz. sonra start next next finish.
------------------------------------------------------------------------------------------------------------------------------

- Böyle bir ekran gelecek tabi sizde hepsi görunmeyecek.
![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/4f51ced3-5180-4d6a-88e5-e0b00fee3914)

- Sunucumuza donuyoruz.
## Sırayla kuralım.
sudo apt update
sudo apt install nodejs
sudo apt install npm
sudo apt install git
## key olusturma işlemleri.
git clone https://github.com/powerpool-finance/powerpool-agent-v2-compose
cd powerpool-agent-v2-compose
npm i
not: sırayla yapıyoruz. ve en son aşağıdaki kodu düzenleyip giriyoruz. %worker_private_key% yerine yeni açtığımız bir metamask cüzdanının private keyini yazıyoruz. %password% kısmınada bir şifre belirliyoruz.
node jsongen.js %worker_private_key% %password%

- sonunda bize bir dosya olusturucak bunu kendi pc mizede yedekliyelim. çünkü lazım olucak :D
/root/powerpool-agent-v2-compose/keys/
yoluna gidiyoruz ve içinde utc ile baslayan dosyayı pcmize kopyalıyoruz.
## my.dappnode sayfamıza geri dönüyoruz.

- tarayıcımızda aşağıdaki adrese gidiyoruz.
- sağ taraftaki advanced optionsa tıklayalım. aşağıdaki resimde göründüğü gibi bypass kısmını aktif ediyoruz. update yazan kısım sizde install yazıcak tıklayın. sonra submit en aşağıya in accept. kurulumun bitmesini bekleyin en son ekrana gelen mesajda enable deyin.
- 
🟪 Prysm Sepolia DAppNode package:
http://my.dappnode/#/installer/%2Fipfs%2FQmT2vSKsKVTs7oFxYnnzb8cpWiKnMDvPLy1qnaLWfEfVkD

![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/2ad33016-f5e5-4a33-883d-c69401ec41ca)

- tekrar tarayıcı adres kısmına

🟫 Geth Sepolia DAppNode package:
http://my.dappnode/#/installer/%2Fipfs%2FQmNy6zTZM9LfHomWJpNYFWX6kJqz9Jgm5eragJagMwc4jk

- sağ taraftaki advanced optionsa tıklayalım. açılan kısımdan show advenced editor ve bypass aktif edelim. sağdan instal diyelim.çıkan ekranda hiç bişi ellemeden submit sonra gelen ekrandan da accept diyelim. kurulum bitince enable diyelim.
- 
![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/5ba59339-0ab2-44ff-92ce-3bd072a5a6e9)

- tekrar tarayıcı adres kısmına (here we go again :D )

![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/4548802f-da10-4f62-aac5-0e7816bdc653)

🟨 PowerAgent DAppNode package:
http://my.dappnode/#/installer/%2Fipfs%2FQmP55bcEhtWtrbiueisuoZx4XN5AeLsuvtKU6CFoTG52GF
- adresine gidelim.sağ taraftaki advanced optionsa tıklayalım. açılan kısımdan bypass aktif edelim. sağdan instal diyelim.
![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/335e3a1f-54ad-4a0f-bb2d-e769b2defdf3)

- gelen ekranda 
worker adress : mm yeni cüzdan olusturup private key almıstık hatırlarsınız. (umarım :D ) onun mm adresini buraya yazıyoruz.
worker keyfile pass: node jsongen.js %worker_private_key% %password% bu kodu duzenlerken olusturduğumuz şifreyi yazıcaz buraya.
Network : sepolia seçiyoruz.
execution clint rpc : ws://sepolia-geth.dappnode:8546
Agent address : 0x4d9bC98452820FD96B2C31741e8C4DdcC795bEce
Accrue reward on poweragent address : true
Execute tasks when block base fee is greater than max base fee : true
Max Priority Fee Per Gas : 60,000
- sumbit diyoruz. yukleme bittikten sonra gelen ekranda enable diyoruz.
- sol kısımdan dashborada geliyoruz.
- ekranda sepolia geth sync olmasını bekliyoruz.
![image](https://github.com/molla202/PowerAgent-Testnet/assets/91562185/1c81c4bb-2fea-41af-985d-fc735ea30a8f)











