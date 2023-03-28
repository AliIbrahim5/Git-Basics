# git_day1

## محتوى الملف
تعريف بالـ Command Line وأساسيات استخدامه.

قراءة الملفات من خلال Command Line.

حذف الملفات باستخدام Command Line.

إنشاء ملفات جديدة باستخدام Command Line.

التعديل على الملفات باستخدام Command Line.

إنشاء مجلّدات جديدة باستخدام Command Line.

حذف المجلّدات باستخدام Command Line.



#### قراءة الملفات من خلال Command Line.

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


#### حذف الملفات باستخدام Command Line.

يمكن حذف الملفات باستخدام Command Line باستخدام أمر "rm" وهو اختصار لـ "remove". يعمل هذا الأمر على حذف الملفات من النظام بشكل دائم، ولا يمكن استرجاع الملفات بعد حذفها باستخدام هذا الأمر.

لحذف ملف باستخدام أمر "rm"، يجب تحديد اسم الملف المطلوب حذفه بالإضافة إلى تمرير الأمر عبر سطر الأوامر. يمكن استخدام الأمر مع خيارات إضافية مثل "-f" لتجاهل أي رسائل تأكيد عند الحذف، أو "-r" لحذف مجلد بأكمله ومحتوياته.

مثال على حذف ملف باستخدام أمر "rm":

    rm filename.txt

في هذا المثال، يتم حذف ملف يحمل اسم "filename.txt" من النظام.

يمكن أيضًا استخدام أمر "rm" لحذف مجلد بأكمله ومحتوياته باستخدام الخيار "-r"، كما في المثال التالي:

    rm -r folder
    لحذف الملجد يجب ان تكون خارج المجلد لكي يتم حذفه
    
في هذا المثال، يتم حذف المجلد "folder" بالإضافة إلى جميع الملفات والمجلدات التي يحتويها. يجب استخدام هذا الأمر بحذر حتى لا يتم حذف ملفات مهمة بطريق الخطأ.



