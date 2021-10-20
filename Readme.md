#  android phone အသုံးပြုပြီး service accounts လုပ်နည်း
## Guide:
- YouTube Link: [Create Service Accounts Tutorial](https://youtu.be/LGWk-UeW4ls)
------
- [x] အရင်ဆုံး Termux ကို မိမိဖုန်းထဲ install လုပ်ပါ။Termux ကို ​အောက်ကပုံ နိပ်ပြီး downloadလုပ်ပါ
[![](credentials/1.png)version 0.117](https://drive.google.com/uc?export=download&id=19VycS90NijIR1u_KYTumRJDu4c2xKK7P)
[![](credentials/2.png)link](https://www.google.com/url?sa=t&source=web&rct=j&url=https://play.google.com/store/apps/details%3Fid%3Dcom.termux%26hl%3Den_US%26gl%3DUS%26referrer%3Dutm_source%253Dgoogle%2526utm_medium%253Dorganic%2526utm_term%253Dtermux%2Bplay%2Bstore%26pcampaignid%3DAPPU_1_sbduYZG9FcvF-gSz3rWYAQ&ved=2ahUKEwjR2bfTutbzAhXLop4KHTNvDRMQ5YQBegQIAxAC&usg=AOvVaw25ySvNLOlqU1oAUA85odtB)

install လုပ်ပီးရင် Termux ကိုဖွင့်လိုက်ပါ
​အောက်က CMD ​တွေ ရိုက်ထည့်ပါ
```
termux-setup-storage
```
```
pkg update
```
```
pkg upgrade 
```
```
pkg install git
```
```
pkg install python
```
```
pip install --upgrade pip
```
```
mkdir /sdcard/MyTermux/ -p
```
```
cd /sdcard/MyTermux
```
```
git clone https://github.com/phoethar1/service-accounts
```
```
cd /sdcard/MyTermux/service-accounts
```
```
pip3 install -r requirements.txt
```
credentials.json file ကို [Google Console](https://console.cloud.google.com/?pli=1)မှာပြုလုပ်ပါ

```
python3 gen_sa_accounts.py --quick-setup -1
```
```
python3 gen_sa_accounts.py  --download-keys Project ID
```
[`Project ID​`](#) နေရာမှာ မိမိ Project IDထည့်

```
python generate_drive_token.py
```
```
cd accounts
```
```
python3 emails.py
```
