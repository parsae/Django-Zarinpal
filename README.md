# Django-Zarinpal
Sample Django ZarinPal WebGate with SOAP--By AParsaee @ SAMAR Web Academy
<h1>«بسم الله الرحمن الرحیم»</h1>
![alt tag](https://raw.githubusercontent.com/aparsaee/Django-Zarinpal/master/Logo.png)![alt tag](https://raw.githubusercontent.com/aparsaee/Django-Zarinpal/master/zarinpal-logo.png)

با سلام و احترام خدمت شما دوستان بزرگوار

برای استفاده از درگاه پرداخت زرین پال به کمک فریمورک جانگو میتوانید از نمونه کد موجود در این پروژه استفاده کنید.این پروژه به زبان پایتون نوشته شده است

<h1>راهنما</h1>

در این پروژه فرض میکنیم که میخواهیم با زدن یک دکمه در یکی از صفحات سایت شما به صفحه اولیه پرداخت زرین پال هدایت شویم.بنابراین باید تعیین کرده باشید که با زدن آن دکمه آدرس زیر فراخوانی شود

<pre><code>urls.py >>> url(r'^request/$', views.send_request, name='request')</code></pre>
آدرس بالا به جانگو فرمان میدهد که از مسیر زیر تابع زیر فراخوانی شود
<pre><code>views.py >>> send_request </code></pre>
از این پس بقیه پردازش ها در سمت وب سرویس زرین پال انجام میشود

وب سرویس زرین پال مقادیری از جمله مرچنت کد، مبلغ و توضیحات را از شما میگیرد و در صورت صحت اطلاعات، شما را به سمت درگاه پرداخت بانک هدایت میکند.ار این پس پرداخت شما موفقیت آمیز باشد یا نباشد یا هر حالت دیگر،پردازش جانگو وارد تابع زیر در مسیر زیر میشود
<pre><code>views.py >>> verify </code></pre>
در تابع فوق حالات مختلف موفقیت یا عدم موفقیت پرداخت شما تعریف شده است که شما میتوانید به دلخواه خود خروجی آن را تغییر دهید

برای کسب اطلاعات بیشتر میتوانید به مستندات فنی اتصال به درگاه پرداخت زرین پال و فیلم های آموزشی سایت زرین پال در آپارات مراجعه فرمایید


موفق و پیروز باشید

پارسائی-آموزشگاه وب ثمر
