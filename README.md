# SE_LAB - آزمایش های درس نرم افزار دانشگاه شریف

**mohammad mahdi behnasr - 97105793**

**reza dolati - 97110411**

***Questions***

<div dir="rtl">

1.هر یک از پنج اصل SOLID را در دو الی سه خط توضیح دهید.

‍‍‍‍‍1. 
 Single Responsibility Principle (SRP): 
 
 هر کلاس و فانکشن باید تنها یک مسئولیت داشته باشد و باید فقط برای انجام آن مسئولیت طراحی شود.

2- Open/Closed Principle (OCP):

 کلاس‌ها باید باز برای توسعه و بسته برای تغییر باشند، به این معنی که باید بتوانیم به راحتی کلاس‌ها را گسترش داده ولی برای تغییر آن‌ها نیاز به تغییر کد قبلی نباشد.

3- Liskov Substitution Principle (LSP):

 هر کلاس فرعی باید قابل جایگزینی با کلاس اصلی خود باشد و همهٔ متد‌های پدر را پشتیبانی کند.



4- Interface Segregation Principle (ISP):

 کلاس‌ها نباید به واسطهٔ وابستگی به اینترفیس‌های زیاد، مجبور به پیاده سازی متدهایی باشند که نیازی به آن‌ها ندارند.



5- Dependency Inversion Principle (DIP):

 وابستگی کلاس‌ها باید به ابسترکسیون‌ها و نه به جزئیات باشد. به عبارت دیگر، باید از ابسترکسیون‌ها برای تعامل با کلاس‌های دیگر استفاده کرد.


--------------------------------
۲.اصول SOLID در کدام یک از گام‌های اصلی ایجاد نرم‌افزار (تحلیل نیازمندی‌ها، طراحی، پیاده‌سازی، تست و استقرار) استفاده می‌شوند؟ توضیح دهید.


اصول SOLID در همهٔ گام‌های ایجاد نرم‌افزار مورد استفاده قرار می‌گیرند. در گام تحلیل نیازمندی‌ها، باید از این اصول برای طراحی سیستم استفاده کرد تا بهترین ساختار برای پاسخ به نیازمندی‌ها را داشته باشیم. در طراحی، باید به این اصول توجه کرد تا ساختار کد مناسب و قابل گسترش را داشته باشیم. در پیاده‌سازی، باید به این اصول توجه کرد تا کد قابل خواندن، قابل نگهداری و قابل توسعه باشد. در تست، باید به این اصول توجه کرد تا تست‌ها به درستی انجام شود و همچنین برای تست‌های واحد، باید از این اصول استفاده کرد. در استقرار، باید به این اصول توجه کرد تا نرم‌افزار به درستی و بدون مشکلات در محیط استقرار شود. به طور کلی، اصول SOLID برای بهبود کیفیت کد و ساختار نرم‌افزار استفاده می‌شوند.
 تعداد زیادی اصول برای مرحله طراحی نرم افزار ها وجود دارد که یکی از آن ها اصول SOLID است.این اصول به این منظور طراحی شده اند که معماری یک برنامه کاربردی را انعطاف پذیرتر، مقیاس پذیرتر و قابل نگهداری تر کنند. اجرای آنها در کار شما می تواند پیچیدگی کلی پروژه را نیز افزایش دهد.

 -----
 ۳.معمولاً گام تست در پایان روند ایجاد نرم‌افزار انجام می‌شود، اما در روش TDD تست‌نویسی پیش از پیاده‌سازی شروع می‌شود. آیا این دو مورد با هم تناقضی دارند؟ توضیح دهید.

 خیر،  در واقع روش TDD با استفاده از تست‌های واحد به 
 طور مداوم کیفیت کد را بررسی می‌کند و همچنین بهبود ساختار نرم‌افزار را تضمین می‌کند. در این روش، قبل از پیاده‌سازی، تست‌های واحد نوشته می‌شود و سپس کد پیاده‌سازی می‌شود. در نهایت، تست‌ها برای اطمینان از عملکرد صحیح نرم‌افزار اجرا می‌شوند. این روش باعث می‌شود که کیفیت کد و ساختار نرم‌افزار بهبود یابد و همچنین تست‌های کامل و جامع برای نرم‌افزار فراهم شود. بنابراین، روش TDD با اصول SOLID همخوانی دارد و بهبود کیفیت کد و ساختار نرم‌افزار را تضمین می‌کند.

هسته TDD نوشتن تست قبل از هر کد تولید است. این اساساً با نحوه انجام کارها در تضاد است. ما می خواهیم کار را سریع به پایان برسانیم و فقط آنچه را که ارسال می شود بنویسیم. ما کد آزمایشی را ارسال نمی کنیم، بنابراین می خواهیم فقط کد نهایی را بنویسیم و با آن کار تمام شود.

تست‌های نوشتاری، توسعه‌دهنده را مجبور می‌کند تا قبل از کدنویسی، یک بار دیگر به تمام الزامات فکر کند، که این چیز خوبی است. اغلب به حذف برخی از فرضیات نامربوط که توسعه‌دهنده ناخودآگاه مطرح کرده‌اند کمک می‌کند. ترجمه الزامات متن به کد اغلب موارد حاشیه ای را نشان می‌دهد که تیم محصول قبلاً به آنها فکر نکرده بود. با این حال، این کار اضافی از . فکر کردن، هنوز هم کار بیشتری بر دوش توسعه دهنده است.

بدون شک TDD سخت است، اما مزایای زیادی دارد. این به ما کمک می کند تا روی نیازمندی ها تمرکز بهتری داشته باشیم، با اطمینان اصلاح کنیم، کد را برای داشتن مسئولیت واحد و رابط های بهتر اجرا کنیم.

------
۴.فرض کنید در آزمایش بالا نیازی به تغییر ابعاد مستطیل نداشتیم. در این حالت طراحی مدل‌ها چه تفاوتی می‌کند؟


در conscructor میتوان مساحت را حساب و از آنجا که طول و عرض تغییر نمیکند پس دیگر نیاز به حساب آن نیست و به فانکشن آن نیازی نداریم 

کلاس setter حذف میشود ، طول و ارض را ابتدا باید در ساخت شی به آن داد  

قابلیت تغییر سایز مستطیل از بین میرود 


</div>
