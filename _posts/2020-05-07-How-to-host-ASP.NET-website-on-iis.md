---
published: true
layout: post
cover-img: 'https://miro.medium.com/max/700/1*MJjTrHkxgJ0F_YfQ4HMsoQ.png'
tags:
  - 'C#'
  - programming
  - iis
subtitle: ''
---

![](https://miro.medium.com/max/700/1*MJjTrHkxgJ0F_YfQ4HMsoQ.png)

ဒီ post လေးကတော့ Junior Level တွေ အတွက်ရည်ရွယ်တာလေးဖြစ်ပါတယ်။ .Net Junior Developer အများစုက ရေးနိုင်ပေမယ် ကိုယ်ရေးထားတဲ့ app ကို အရင်ဆုံး localhost မှာတင် IIS နဲ့ဘယ်လို host လို့ရမယ်မှန်း မသိကြတာများပါတယ် အဲအတွက် လေ့လာစမ်းချင်တဲ့ junior level တွေကို ရည်ရွယ်ထားတာပါ။

## What is IIS?
IIS ရဲ့ အရှည်ကောက်ကတော့ Internet Information Services ပါ့ web server တမျိုးပေါ့ ကျနော်တို့ ရေးတဲ့ ASP.Net application တွေဟာ IIS ပေါ်မှာပဲ run တာပါ။ php ဆိုရင် apche server ပေါ်မှာ run တာပေါ့ အဲလိုမျိုး language ပေါ် မူတည်ပြီး ကွဲတာပါ။ IIS ကတော့ Window OS တွေမှာ ပါပြီးသားပါ programs and features ကနေ ထပ်ဖွင့်ပေးရုံပါပဲ။

## How to turn on IIS?
Window မှာ IIS တွေက ဖွင့်ထားပြီးသားမရှိပါဘူး program and feature ကနေ သွားဖွင့်ပေးရပါတယ်။ အရင်ဆုံး ကိုယ်စက်ထဲမှာဖွင့်ပြီးသားလား သိရအောင် Run >>ကနေ inetmgr ရိုက်ဖွင့်ကြည့်ပါ error ပဲ တတ်လာရင်တော့ မရှိသေးပါဘူး ကျနော်တို့ window search box ကနေပဲ programs and features လို့ရှာပြီးဖြစ်ဖြစ် control panel ကပဲဖြစ်ဖြစ် programs and features ကိုသွားလိုက်ပါ အဲကနေ Turn Windows features on or off ကို ဖွင့်လိုက်ပါ။

![Turn on IIS at Programs and Features](https://miro.medium.com/max/700/1*XSbWtDgNgHBmd2nv7WoQQg.jpeg)

Windows Features popup လေးတတ်လာရင် Internet Information Services ကို အမှန်ဖြစ်ပြီး ok နှိပ်ပြီး apply လုပ်လိုက်ပါ။ နည်းနည်းတော့ စောင့်ရပါမယ် install လုပ်လို့ပြီးပီး ဆိုရင်တော့ Run ကနေတဆင့် inetmgr လို့ရိုက်ဖွင့်လို့ရပါပီ အဆင်ပြေတယ်ဆိုရင်တော့ အောက်ကပုံအတိုင်းလေး တတ်လာပါလိမ့်မယ်။

![Internet Information Services (IIS) Manager](https://miro.medium.com/max/700/1*J6ciyheyh9IUgSoA9idAFA.jpeg)

## How to host ASP.Net Application on IIS?
IIS မှာ host လုပ်ဖို့ဆို ကျနော်တို့ ရေးထားတဲ့ project ကိုအရင်ဆုံး publish လုပ်ပေးရပါမယ်။ ကျနော်တို့Visual Studio မှာ project name ကို right click ကနေ Publish နှိပ်လိုက်ပါ။

![Publish project 1](https://miro.medium.com/max/700/1*3wO9WkKMlVYDW9uZ9Tc0Xw.jpeg)

Publish Web popup လေးတတ်လာပါမယ်။ Profile ဆိုတာကတော့ ကျနော်တို့ project တခုတွက် profile တခုထားထားပေးပြီး နောက်ထပ်တခါ ဒီ project ကိုပဲ ထပ်ပြင်ထားလို့ host လုပ်ထားတဲ့ဆီကို update လုပ်ချင်ရင် setting တွေ publish path folder တွေ ပြန်ရွေးစရာမလိုပဲ သိမ်းထားလို့ရအောင်ပါ New Profile ကနေ HelloWorld ဆိုပြီး profile တခု ဆောက်လိုက်ပါ။

Profile ဆောက်ပြီးပီ ဆိုရင်တော့ ကျနော်တို့ Connection အပိုင်းမှာ Publish method ရွေးရပါမယ် အဲမှာ File System ကိုပဲ ရွေးပါမယ် FTP ကတော့ online ပေါ်တင်တဲ့အခါမျိုးမှာ အဆင်ပြေပါတယ် နောက်မှ online ပေါ် တင်တဲ့ post တခုထပ်ရေးပါမယ်။

ကျနော်တို့ File System ရွေးထားတဲ့အတွက် ကျနော်တို့ project publish လုပ်လိုက်ရင် ထားမယ် folder path ကို D Drive ထဲမှာဖြစ်ဖြစ် folder အသစ်တခု သီးသန့်ဆောက်ပြီး Target location မှာ ရွေးပေးပါ။ ပြီးရင်တော့ ကျနော်တို့ Publish လုပ်လို့ရပါပြီ။Publish လုပ်ပြီးသွားရင် ကျနော်တို့ရွေးထားတဲ့ folder path မှာ project file တွေထက်လာပါမယ်။ နောက်ထပ် ကျနော်တို့IIS မှာ ဒီ folder path နဲ့ website တခု သွားဆောက်ပေးရပါမယ်။

![Publish project 2](https://miro.medium.com/max/700/1*9egxKu0iRWvqyzJ6XDhq0w.jpeg)

IIS မှာ Sites ကို Right click နှိပ်ပြီး Add Website လုပ်ပါ။ popup တတ်လာရင်တော့ Site name မှာ project name ဖြစ်ဖြစ် ပေးလိုရပါတယ် physical path မှာတော့ ခုနက publish လုပ်ထားတဲ့ folder path ကိုရွေးပေးလိုက်ပါ။ Port ကိုလည်း ၄လုံး ဒါမှ မဟုတ် ၂ လုံး မိမိနှစ်သက်ရာ ပေးလို့ရပါတယ် ကျန်တာတော့ ပုံထဲက အတိုင်းရွေးပြီး OK နှိပ်လိုက်ရင် IIS ပေါ်မှာ application ကို host ပြီးသွားပါပီ။

![Add Website on IIS](https://miro.medium.com/max/700/1*JQPP6WEpVO5gW4tkrgnWKw.jpeg)

## How to run hosted website on IIS?
IS မှာ website ထဲလို့ပြီးသွားရင်တော့ ကျနော်တို့ browser ကနေ localhost ရယ် port number ရယ် သုံးပြီး ဖွင့်လို့ရပါပီ။ ဥပမာ localhost:8080 ပါ။ ဒါဆိုရင် ကျနော်တို့project ကို Visual Studio ကနေ run စရာမလိုတော့ပဲ localhost:8080 ဆိုပြီးပဲ ဖွင့်ကြည့်လို့ရပါပြီ။ တခြားစက်ကနေလည်း same network ဆိုပြီး ဖွင့်ကြည့်လို့ရပါတယ်။

ဥပမာ host လုပ်ထားတဲ့စက် IP က 192.168.1.1 ဆိုရင် တခြား network တူတဲ့စက်ကနေ localhost နေရာမှာ 192.168.1.1:8080 ဆိုပြီး browser ကနေပဲ ဖွင့်ကြည့်လို့ရပါတယ်။

![](https://miro.medium.com/max/700/1*_L54vJ8pR5Xh2ni8qfdEfQ.jpeg)

project က database connection ရှိရင်တော့ အောက်မှာပြထားတဲ့ ပုံအတိုင်း error တတ်နိုင်ပါတယ်။

![](https://miro.medium.com/max/700/1*qcJl4wsCmlzEVG54WtI1Jg.jpeg)

စိတ်မပူပါနဲ့ဒါက ကျနော်တို့ IIS မှာ host လုပ်ထားတဲ့ application က DB connection ယူတဲ့အခါမှ login permission မရှိလို့ပါ။ အဲတော့ MSSQL မှာ database မှာ user တခု သွားထည့်ပေးရပါမယ်။ Login failed for user ‘IIS APPPOOL\DefaultAppPool’ ဖြစ်တဲ့အတွက် database မှာ IIS APPPOOL\DefaultAppPool နာမည်နဲ့user တခု အောက်ကပုံမှာ ပြထားတဲ့အတိုင်း ထည့်ပေးရပါမယ်။


![](https://miro.medium.com/max/700/1*GyVzWbIrwlQnCzlBHLIADA.jpeg)

![](https://miro.medium.com/max/699/1*ZZ6veTb9yES7iVGcRVwHQg.jpeg)

![](https://miro.medium.com/max/693/1*g7JdwHfkzNvN1pTlO4nu-g.jpeg)

![](https://miro.medium.com/max/689/1*K6inQZvxrikR-YhAOgufSA.jpeg)

ပုံထဲက အတိုင်း Login Name နဲ့ permission တွေရွေးပြီးရင်တော့ DB connection ယူတဲ့နေရာမှာ error မရှိတော့ပါဘူး။ ပြန်စမ်းကြည့်လို့ရပါပြီ။ same network မှာ တခြားစက်နေ ဖွင့်ရင် Windows firewall ကြောင့် ဖွင့်မရတတ်တာမျိုးရှိပါတယ်။ အဲအခါကျ firewall ပိတ်တာပဲဖြင့်ဖြင့် application host လုပ်ထားတဲ့ port number 8080 ကိုဖွင့်ပေးတာဖြစ်ဖြစ်လုပ်ပြီးရင် ကြည့်လို့ရပါတယ်။

ဒီနည်းနဲ့ကတော့ အများအားဖြင့် ရုံးတွင်းပဲ သုံးပြီး online internet ပေါ်မတင်တဲ့ webbased software တွေကို သုံးတဲ့နေရာမှာ သုံးကြပါတယ်။ ရုံးထဲမှာ ဆာဗာကောင်းကောင်းတလုံးနဲ့software application တလုံးကို IIS ပေါ်မှာ host ထားပေးလိုက်ရင် HR software ဖြစ်ဖြစ် တခြားဟာဖြစ်ဖြစ် ရုံးတွင်းပိုင်းမှာပဲ same network အနေပဲသုံးလို့ရနေပါလိမ့်မယ်။
