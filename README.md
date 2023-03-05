# -RAT-Telegram
RAT عبر Telegram





أداة إدارة Windows عن بعد عبر Telegram (الآن في Python 3.7!) | تم إنشاؤه في الأصل بواسطة https://t.me/jokerplstaeen


![image](https://user-images.githubusercontent.com/107787017/222980497-0a06f05d-875d-4c9c-bb7c-27bd2fa3081c.png)




لماذا واحد آخر؟
تواجه أدوات الإدارة عن بُعد الحالية في السوق مشكلتين رئيسيتين:



نقص التشفير.
تتطلب إعادة توجيه المنفذ من أجل التحكم من مئات الأميال.
يتغلب RAT على هاتين المشكلتين باستخدام Telegram bot API.


مشفر بالكامل. لا يمكن التجسس على البيانات التي يتم تبادلها عند استخدام أدوات MITM.
يوفر تطبيق Telegram messenger طريقة بسيطة للتواصل مع الهدف دون تكوين المنفذ للأمام قبل تسليم الهدف.




________________________________________________________________________________________________________________________________________________________________________________


سمات:



تم تضمين Keylogger مع سجل عنوان النافذة
احصل على إصدار Windows الخاص بجهاز الكمبيوتر المستهدف والمعالج والمزيد
احصل على معلومات عنوان IP للكمبيوتر الهدف والموقع التقريبي على الخريطة

حذف ونقل الملفات

إظهار الدليل الحالي

تغيير الدليل الحالي

سرد الدليل الحالي أو المحدد

قم بتنزيل أي ملف من الهدف

تحميل الملفات المحلية إلى الهدف. أرسل صورتك أو pdf أو exe أو أي شيء يتعلق fileببوت Telegram

تشغيل تلقائي لتشغيل مقطع فيديو في وضع ملء الشاشة ولا توجد عناصر تحكم لمقطع فيديو youtube على الهدف
خذ لقطات

نفّذ أي ملف

الوصول إلى الميكروفون

ابدأ تشغيل خادم وكيلHTTP

تجميد لوحة المفاتيح الهدف  

جدولة المهام للتشغيل في التاريخ والوقت المحدد  

تشفير / فك جميع الملفات المحلية

أهداف بينغ

تحديث exe. - شكرًا AHM7D Sy

RAT التدمير الذاتي
تغيير الخلفية من ملف أو عنوانurl

قم بتنفيذ قذيفة cmd


أخذ لقطات من كاميرا الويب (إذا كانت مرفقة)
قم بتنفيذ لعبة python 3.7 عشوائية أثناء التنقل

تجميد الماوس الهدف


[TODO] المتصفح (IE ، Firefox ،كروم) استرجاع ملفات تعريف الارتباط

[TODO] استرجاع كلمة المرور

[TODO] مراقبة حركة مرور الويب (بيانياً؟)

[TODO] مراقبة النطاق الترددي (نقطة انطلاق لمراقبة حركة مرور الويب) - بدأت في 28/10/2018

[TODO] صقل البرمجة النصية (على سبيل المثال: إذا تم فتح التطبيق x ، فسيتم تنفيذ y)

[TODO] التقاط الحافظة (نص ، صورة)

[TODO] إخفاء رموز سطح المكتب

[TODO] ضغط الصوت

[TODO] البحث عن خادم الأسماء (/ nslookup - # 19 )


لقطات


![ششش](https://user-images.githubusercontent.com/107787017/222980705-70f43b84-281b-42b9-aeba-05e034414a69.PNG)


![ءءء](https://user-images.githubusercontent.com/107787017/222980725-8d01625e-5ee0-4367-b59c-291b85ab9d4e.PNG)


Installation & Usage:

Clone this repository.

Set up a new Telegram bot talking to the BotFather.

Copy this token and replace it in the beginning of the script.

Run compile.py

Generates an executable binary

To run the script: python RATAttack.py.

Find your bot on telegram and send some command to the bot to test it.

To restrict the bot so that it responds only to you, note down your chat_id from the console and replace it in the script and comment out the line return True. Don't worry, you'll know when you read the comments in the script.








الأوامر:
عند استخدام الأوامر أدناه ؛ تستخدم /كبادئة. على سبيل المثال /pc_info:.



arp - display arp tableط

capture_pc - screenshot PC

cmd_exec - execute shell command

cp - copy files

cd - change current directory

delete - delete a file/folder

download - download file from target

decode_all - decode ALL encoded local files

dns - display DNS Cache

encode_all - encode ALL local files

freeze_keyboard - enable keyboard freeze

unfreeze_keyboard - disable keyboard freeze

get_chrome - Get Google Chrome's login/passwords

hear - record microphone

ip_info - via ipinfo.io

keylogs - get keylogs

ls - list contents of current or specified directory

msg_box - display message box with text

mv - move files

pc_info - PC information

ping - makes sure target is up

play - plays a youtube video

proxy - opens a proxy server

pwd - show current directory

python_exec - interpret python

reboot - reboot computer

run - run a file

schedule - schedule a command to run at specific time

self_destruct - destroy all traces

shutdown - shutdown computer

tasklist - display services and processes running

to - select targets by it's name

update - update executable

wallpaper - change wallpaper



تجميع:

كيفية التحويل البرمجي:

تشغيل compile.py. يمكنك أيضًا المرور --icon=<path/to/icon.ico>لاستخدام رمز مخصص. إذا كنت تريد استخدام UPX للضغط ، فيمكنك الإضافة --upx-dir [upx-3.95-win64 | upx-3.96-win32]، اعتمادًا على البنية الخاصة بك. يمكنك تخطي هذا الخيار الأخير إذا كان لديك UPX في PATHمتغير البيئة الخاص بك.
بمجرد أن يتم تجميعه بنجاح ، ابحث عن .exeالملف في C:/Python37/Scripts/dist/أو الدليل الحالي ، اعتمادًا على المكان الذي اتصلت منه منه.
حذار! إذا قمت بتشغيل المترجم .exe، سينتقل البرنامج النصي نفسه لبدء التشغيل والبدء بجهاز الكمبيوتر الخاص بك للتشغيل عند بدء التشغيل. يمكنك العودة إلى الوضع الطبيعي باستخدام /self_destructالخيار أو إزالة %APPDATA%/Portalالدليل و %APPDATA%/Microsoft/Windows/Start Menu/Programs/Startup/portal.lnk.
تعديل الإعدادات:

يمكنك أيضًا تعديل اسم .exeالملف المخفي وموقعه واسم المجلد الذي .exeسيخفي فيه المخفي نفسه. لفعل هذا؛ تعديل compiled_nameو hide_folderعلى التوالي.
قم بتعيين معرفات الدردشة المعروفة لبداية RATAttack.py  


المساهمة: 


لا يزال هذا المشروع في مراحله المبكرة ، لذا يمكنك توقع بعض الأخطاء. لا تتردد في الإبلاغ عنها! والأفضل من ذلك ، أرسل طلب سحب :)
أي ميزات وأفكار جديدة موضع ترحيب كبير! يرجى تقديم طلبات الميزات من خلال إنشاء المشكلات
تم تمكين حماية الفرع master. يجب أن تعمل في فرع بديل (على سبيل المثال dev) وتقوم بعمل علاقات عامة. هذا للتأكد من أن السيد لديه نسخة صالحة للعمل ومعتمدة من RvT.



للتبرع لي 



Bitcoin: 1EgF4hzUcvxcHdXvEN59kdWRSzZZ1Uq1G9 

 
