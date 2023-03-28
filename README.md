# تعريف بالـ Command Line وأساسيات استخدامه.



## محتوى الملف
تعريف بالـ Command Line وأساسيات استخدامه.
- قراءة الملفات  
- حذف الملفات  
- إنشاء ملفات جديدة  
- التعديل على الملفات  
- إنشاء مجلّدات جديدة  
- حذف المجلّدات  .



#### قراءة الملفات  

يتيح استخدام سطر الأوامر (Command Line) للمستخدمين قراءة محتوى الملفات بسهولة دون الحاجة إلى استخدام واجهة رسومية. يمكن استخدام الأوامر المختلفة لقراءة ملفات النص العادية وملفات أخرى مثل الصور وملفات الصوت.

لقراءة محتوى ملف نصي باستخدام أمر "cat"، يمكنك كتابة الأمر التالي:

    cat filename.txt


حيث يتم استخدام "filename.txt" لتحديد الملف الذي تريد قراءته. ستتم طباعة محتوى الملف مباشرة على سطر الأوامر.

لقراءة الملفات الطويلة التي تتجاوز طول الصفحة، يمكن استخدام أمر "more" بدلاً من "cat". يمكن استخدام الأمر التالي:

    more filename.txt
    
    

يمكن استخدام أمر "less" لقراءة الملفات بطريقة مماثلة لأمر "more"، ولكن يوفر أيضاً خيارات إضافية مثل البحث عن كلمات معينة في الملف. يمكن استخدام الأمر التالي:


     less filename.txt
     
    بعد كل صفحة، سيتم انتظار المستخدم للاستمرار في القراءة. ويمكن استخدام "q" للخروج من الأمر.

بعد الدخول إلى الأمر، يمكن استخدام "q" للخروج، أو "/word" للبحث عن كلمة محددة، أو "n" للانتقال إلى الظهور التالي للكلمة المبحوثة.


#### حذف الملفات

يمكن حذف الملفات باستخدام Command Line باستخدام أمر "rm" وهو اختصار لـ "remove". يعمل هذا الأمر على حذف الملفات من النظام بشكل دائم، ولا يمكن استرجاع الملفات بعد حذفها باستخدام هذا الأمر.

لحذف ملف باستخدام أمر "rm"، يجب تحديد اسم الملف المطلوب حذفه بالإضافة إلى تمرير الأمر عبر سطر الأوامر. يمكن استخدام الأمر مع خيارات إضافية مثل "-f" لتجاهل أي رسائل تأكيد عند الحذف، أو "-r" لحذف مجلد بأكمله ومحتوياته.

مثال على حذف ملف باستخدام أمر "rm":

    rm filename.txt

في هذا المثال، يتم حذف ملف يحمل اسم "filename.txt" من النظام.

يمكن أيضًا استخدام أمر "rm" لحذف مجلد بأكمله ومحتوياته باستخدام الخيار "-r"، كما في المثال التالي:

    rm -r folder
    لحذف الملجد يجب ان تكون خارج المجلد لكي يتم حذفه
    
في هذا المثال، يتم حذف المجلد "folder" بالإضافة إلى جميع الملفات والمجلدات التي يحتويها. يجب استخدام هذا الأمر بحذر حتى لا يتم حذف ملفات مهمة بطريق الخطأ.


####  إنشاء ملفات جديدة  

يمكن إنشاء ملفات جديدة باستخدام Command Line باستخدام أمر touch في معظم أنظمة التشغيل. يقوم الأمر بإنشاء ملف جديد إذا لم يكن موجودًا، أو تحديث تاريخ آخر تعديل للملف إذا كان موجودًا بالفعل.


لإنشاء ملف جديد، يتم استخدام الأمر touch مع اسم الملف المطلوب إنشاؤه. على سبيل المثال، يمكن استخدام الأمر التالي لإنشاء ملف جديد يحمل اسم "newfile.txt":

    touch newfile.txt


إذا كان الملف غير موجود بالفعل، فسيتم إنشاء الملف وتحديث تاريخ آخر تعديل له. وإذا كان الملف موجودًا بالفعل، فسيتم تحديث تاريخ آخر تعديل للملف فقط.

يمكن أيضًا استخدام الأمر echo لإنشاء محتوى في الملف المنشأ حديثًا. على سبيل المثال، يمكن استخدام الأمر التالي لإنشاء ملف جديد وإضافة بعض النص إليه:

    echo "Hello, World!" > newfile.txt


ستتم إضافة النص "Hello, World!" إلى الملف الجديد "newfile.txt". يمكن استخدام برامج تحرير النصوص مثل Vim أو Nano لتعديل المحتوى في الملف.

يتم إنشاء الملفات الجديدة في الدليل الحالي (المجلد) الذي يعمل فيه Command Line. ويمكن استخدام الأمر "cd" للتنقل بين المجلدات والتأكد من مكان إنشاء الملف.


#### التعديل على الملفات 

يمكن التعديل على الملفات باستخدام سطر الأوامر (Command Line) باستخدام أمر المحررات النصية مثل Nano و Vim و Emacs أو باستخدام أوامر التحرير المدمجة في نظام التشغيل مثل sed و awk.

لتحرير ملف باستخدام محرر النصوص Nano، يمكن استخدام الأمر التالي:

    nano file.txt



سيتم فتح الملف "file.txt" في محرر النصوص Nano، ويمكن تعديل المحتوى وحفظ التغييرات باستخدام الاختصارات الموجودة في الأسفل.



بالإضافة إلى ذلك، يمكن استخدام أمر sed لتعديل الملفات من سطر الأوامر. على سبيل المثال، لتعديل ملف يحتوي على النص "welcome to javascript " إلى "welcome to python "، يمكن استخدام الأمر التالي:


     sed -i 's/javascript/python/g' file.txt


#### إنشاء مجلّدات جديدة 

يمكن إنشاء مجلدات جديدة في نظام التشغيل باستخدام أدوات سطر الأوامر (Command Line) بسهولة. يتم استخدام أمر "mkdir" لإنشاء مجلد جديد، ويتم تمرير اسم المجلد كمعامل للأمر.

لإنشاء مجلد جديد باستخدام الأمر "mkdir"، يتم اتباع الخطوات التالية:

1- افتح نافذة سطر الأوامر (Command Prompt) أو نافذة تطبيق الطرفية (Terminal) حسب نظام التشغيل الذي تستخدمه.

2- انتقل إلى المجلد الذي تريد إنشاء المجلد الجديد فيه باستخدام أمر "cd"، على سبيل المثال:

      cd Documents
3- استخدم الأمر "mkdir" مع اسم المجلد الجديد الذي تريد إنشاؤه، على سبيل المثال:

      mkdir my_folder

بعد تنفيذ هذه الخطوات، سيتم إنشاء مجلد جديد يحمل الاسم "my_folder" في المجلد الحالي.





