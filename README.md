# قالب اختصاصی مرزبان و مرزنشین اورانوس | Ourenus

## Desktop View
<img width="1458" alt="image" src="https://github.com/user-attachments/assets/49983ceb-fefd-4a35-a488-4202dc7bd353">



## Responsive Mobile View
![image](https://github.com/user-attachments/assets/9a0605e4-f339-4a79-86f5-5aadd4fee9d9)




---

## ساخته شده توسط
- **React**: Version 18
- **Vite**: Version 5
- **Material UI**

---

## ویژگی ها
- **اپلیکیشن ها**: لیست اپلیکیشن های قابل تغییر و توسعه
- **اطلاعات کاربر**: اطلاعات سرویس کامل و کاربردی
- **مدیریت کانفیگ**: دریافت لیست کانفیگ ها و دریافت بارکد هر کانفیگ
- **دو زبانه**: پشتیبانی از زبان انگلیسی و فارسی
- **شخصی سازی**: قابلیت شخصی سازی رنگ ها و تم 

---

## مراحل نصب

### مرزبان

۱. **قالب رو با دستور زیر دانلود کنید**
   ```sh
   sudo wget -N -P /var/lib/marzban/templates/subscription/ https://github.com/MatinDehghanian/Ourenus/releases/latest/download/index.html
   ```

۲. **دستورات زیر رو تو ترمینال سرورتون بزنید**
   ```sh
   echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
   echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
   ```
   یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` با پاک کردن `#` اول آنها از حالت کامنت در بیارید.
   ```
   CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
   SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
   ```

۳. **ریستارت کردن مرزبان**
   ```sh
   marzban restart
   ```

### مرزنشین

۱. **قالب رو با دستور زیر دانلود کنید**
   ```sh
   sudo wget -N -P /var/lib/marzneshin/templates/subscription/ https://github.com/MatinDehghanian/Ourenus/releases/latest/download/index.html
   ```

۲. **دستورات زیر رو تو ترمینال سرورتون بزنید**
   ```sh
   echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"' | sudo tee -a /etc/opt/marzneshin/.env
   echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /etc/opt/marzneshin/.env
   ```
   یا مقادیر زیر رو در فایل `.env` در پوشه `/etc/opt/marzneshin` با پاک کردن `#` اول آنها از حالت کامنت در بیارید.
   ```
   CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzneshin/templates/"
   SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
   ```

۳. **ریستارت کردن مرزنشین**
   ```sh
   marzneshin restart
   ```

---

## بروزرسانی قالب
برای بروزرسانی تمپلیت فقط کافیست مرحله 1 را تکرار کنید.

---

## شخصی سازی
برای شخصی سازی لیست اپلیکیشن ها و لیست پشتیبانی:
- **اپلیکیشن ها**: [public-assets Apps JSON](https://github.com/MatinDehghanian/public-assets/blob/main/json/apps.json)
- **توضیحات**: ریپازیتوری من رو فورک کنید. و باتوجه به ساختار اون لینک یا اسم یا عکسش رو تغییر بدید

**ویدیو آموزشی**:  
[![YouTube Tutorial Video](https://img.youtube.com/vi/l5Pvy6Hof9o/0.jpg)](https://www.youtube.com/watch?v=l5Pvy6Hof9o)
[![YouTube Tutorial Video #2](https://img.youtube.com/vi/6s8931r9E24/0.jpg)](https://youtu.be/6s8931r9E24)

---

## حمایت و سفارشات
برای پشتیبانی یا سفارش قالب اختصاصی با من توی تلگرام در ارتباط باشید [Telegram](https://t.me/Mqtin).

<a href="https://nowpayments.io/donation?api_key=Z50AKDD-DHSMN86-P0DQ22X-1SQAFCA" target="_blank" rel="noreferrer noopener">
    <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>

