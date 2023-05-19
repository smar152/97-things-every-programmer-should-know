# از ساختارشکنی نترسید!

کمتر کسی را می‌توان یافت که در حوزه ی برنامه نویسی کار کرده باشد و با پروژه یی مواجه نشده باشد که ساختار کدنویسی آن مشکل داشته باشد. در چنین پروژه هایی، رفع یک باگ منجر به ایجاد ده‌ها باگ دیگر خواهد شد! در چنین شرایطی، برنامه نویس کاملاً دست به عصا کدنویسی کرده و همیشه این نگرانی را دارد که پروژه از هم بپاشد.

دلیل مواجهه با چنین مشکلی کاملاً واضح است و این دلیل چیزی نیست جز «بیمار» بودن سیستم و این بیمار نیاز به یک پزشک دارد و در غیر این صورت، اوضاع از این هم وخیم تر خواهد شد. در‌ واقع، همان‌طور که یک عمل جراحی در ابتدا با درد همراه است و شرایط اصلاً خوشایندی را برای بیمار فراهم نمی کند اما در نهایت منجر به سلامت بیمار می شود، در این گونه پروژه ها نیز می بایست متحمل چنین دردی شویم!

خود شما –به عنوان برنامه نویس یا یکی از برنامه نویسان چنین پروژه یی- دقیقاً می‌دانید که مشکل از کجا است و چه بخش‌هایی نیاز به ریفکتور شدن دارند اما از دست به عمل شدن هراس دارید.

به خاطر داشته باشید به طور خلاصه، منظور از Code Refactoring (کد ریفکتورینگ) این است که ساختار فعلی سورس کد یک پروژه را تغییر دهیم -یا بهتر بگوییم بهبود بخشیم- بدون آن که تاثیری در نوع ماهیت پروژه ایجاد گردد. فرض کنیم چند سال پیش کدی را نوشته ایم، حال که چیزهای جدید فرا گرفته ایم و به کد نگاه می کنیم، می بینیم کدی که مثلا در 40 خط نوشته ایم را می توان خیلی بهینه تر کرده و به 10 خط کاهش داده و در عین حال اثربخشی آن را نیز بیشتر کرد. به چنین کاری Refactoring گفته می شود.
مادامی که شما به صورت لوکال اقدام به تغییر و تحول سورس کد خود می کنید، هرگز از دست کاری کد خود نترسید چرا که در نهایت منجر به بهبود وضعیت پروژه خواهد شد. خیلی از اوقات ما -به عنوان برنامه نویس- می‌دانیم که مشکل از کجا است اما یا حوصله ی رفع کردن آن را نداریم یا به دلیل طولانی شدن زمان کار کردن روی پروژه، ترجیح می‌دهیم مشکلات را به حال خود رها کرده و روی پروژه ی دیگری کار کنیم و یا این که از رو به رو شدن با مشکلات پروژه هراس داریم.

متأسفانه خبر بد این که این شتری است که درب خانه ی هر برنامه نویسی می خوابد! شما چاره یی جز این ندارید که سورس کد خود را ریفکتور کنید، باگ ها را رفع کنید و وابستگی‌ها را به حداقل برسانید. اگر هم روی پروژه یی کار می‌کنید که شما مسئول مستقیم آن نیستید، سعی کنید مدیر خود را مجاب کنید که اگرچه این اصلاحات نتایج ملموس و قابل مشاهده یی ایجاد نمی کنند، اما در نهایت منجر به کاهش هزینه‌ها در دراز مدت و تجربه ی کاربری بهتری می شوند.

به خاطر داشته باشید Dependency (دیپندنسی یا وابستگی) در توسعه ی نرم افزار به این نکته اشاره دارد که سورس کد پروژه ما برای اجرای تمام و کمال، نیاز به سایر کدها، لایبرری ها و حتی سایر نرم افزارها داشته باشد. توجه داشته باشیم که در توسعه ی نرم افزار، می بایست تمام تلاش خود را به کار بندیم تا این وابستگی ها به حداقل برسند. علاوه بر این، اصطلاحی داریم تحت عنوان Dependency Hell یا «جهنم وابستگی» که وقتی رخ می دهد که نرم افزار ثالثی که از آن در پروژه ی خود استفاده می کنیم تغییری در سورس کد اش ایجاد می کند که این تغییر منجر به عملکرد ناصحیح نرم افزار ما خواهد شد.