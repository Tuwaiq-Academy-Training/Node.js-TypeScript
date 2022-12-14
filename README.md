##  محتوى اليوم الثاني

محتوى الملف:

- ماهو node.js
- ماهو npm
- تثبيت node & npm
- كيفية تثبيت مكتبة من npm
- الاوامر المستخدمة في npm
- ما هي TypeScript
- تثبيت وإعداد  TypeScript
- أهم مزايا TypeScript 


 ## ماهو node.js
 
من المعروف بأن لغة الجافا سكربت هي لغة الClient Side، بمعنى ذلك انها لغة تعمل بجانب المستخدم وليس في السيرفر ولكن بعد تطوير ريان دال لهذا الباترن (النود جي اس) الذي يعمل بمحرك قوقل V8 والعديد من الlibraries الاخرى اصبح الامر اكثر تعقيدا من ذي قبل و تحول هذا الإطار بالعمل في السيرفر كمثل الPHP، بمعنى اخر، الNode.js اصبح إطار عمل Functionality حركية و ديناميكية بشكل تام بإمكانك التعامل مع قواعد البيانات وما الى ذلك من خلاله بكل سهوله.

 
#### كيفية عمل node.js

يستخدم إطار الNode.js لبرمجة تطبيقات الويب بالتحديد و المواقع بشكل عام، يعتمد في عمله على الevents او باللغة العربية تدعى ( المناسبات )  لذلك اي شي يحصل على السيرفر يقوم بإطلاق non-blocking event كل كونكشن جديد => fires event ، معلومات مرسله من فورم => fires event ، طلب بيانات من قاعدة البيانات من قبل المستخدم => fires event.

عمليا، هذا يعني ان الموقع او التطبيق لا يمكن ان يتاخر بتنفيذ مناسبة event حتى لو دخله او استخدمه آلاف المستخدمين في نفس الوقت لان إطار ال Node.js برمج ليكون Non-Blocking بذلك الأوامر يتم تنفيذها بالتوازي بخلاف الPHP التي هي لغة block until completion اي ان الاوامر لايتم تنفيذها الا بتنفيذ ما سبق من اوامر وهذا هو الفرق الاكبر مابين PHP & Node.js وهذا هو سبب تميز إطار عمل النود وسبب السرعه الرهيبه في تنفيذ الاوامر.
 
 ## ما هو npm
  اختصار لـ Node Package Manager هو نظام إدارة الحزم خاص بلغة javascript  .

نحتاج نظام npm  عندما نعمل على مشاريع javascript  كما انه المدير الرئيسي لبيئة Node.js. 

يتكون مدير الحزم npm  من واجهة  أوامر يستعملها المستخدم  وقاعدة بيانات على الإنترنت، تدعى "مخزن npm". يتم الوصول إلى هدا المخزن عن طريق المستخدم عن طريق برنامج سطر الأوامر  الدي يمكنه من تصفح مختلف الحزم والبحث عنها على الموقع الرسمي لمجمع [npm](https://www.npmjs.com)

## تثبيت node & npm

- قم بتنزيل node من الموقع الرسمي   [NodeJS WebSite](https://nodejs.org/en/)

#### الخطوة 1 :نقوم بتنزيل برنامج التثبيت
![image](https://user-images.githubusercontent.com/92247967/199274690-0eb48ccc-f63d-4762-9b3b-a36aa6f9c266.png)

#### الخطوة 2: نقوم بتثبيت كل من node وnpm
![image](https://d2ms8rpfqc4h24.cloudfront.net/Install_NPM_and_Node_js_dfb6f2ff29.png)

#### الخطوة 3: اختر المسار المطلوب حيث تريد تثبيت node.js

![image](https://d2ms8rpfqc4h24.cloudfront.net/uploads/2021/10/Choose-Path-to-Install-Node.js.png)

####  بعد ذالك سيتم تثبيت المزايا التالية افتراضيا 
![image](https://d2ms8rpfqc4h24.cloudfront.net/Select_Node_js_Features_to_install_0847ad9e3a.png)

#### بعد الضغط على التالي ستظهر صفحة التثبيت ونقوم بتثبيت المزايا
![image](https://d2ms8rpfqc4h24.cloudfront.net/uploads/2021/10/Final-Step-of-Node.js-Installation.png)

#### واخيرا ! لتحقق من الاصدار المثبت لدينا نقوم بفتم التيرمنال(cmd)
- اصدار npm

          npm -v
          
- اصدار node      

          node -v
    
![image](https://d2ms8rpfqc4h24.cloudfront.net/uploads/2021/10/Frequent-Update-of-Node-and-NPM.png)

##  كيفية تثبيت مكتبة من npm

#### تنزيل الحزم وتثبيتها محليًا
دائمًا ما تكون الحزم التي لم يتم فحصها عامة ، مما يعني أنه يمكن البحث عنها وتنزيلها وتثبيتها بواسطة أي شخص. لتثبيت حزمة عامة ، في سطر الأوامر ، قم بتشغيل
       
       npm install <package_name>
       
       
## بعض من الاوامر المستخدمة في npm

| الاوامر  | الخصائص |
|:---:|:------:|
|  npm -v   |استخدم هذا الأمر لطباعة إصدار |--- |
|  npm init  |يؤدي استخدام "npm init" من سطر الأوامر إلى تهيئة ملف package.json الخاص بالمشروع|
| npm install <اسم الحزمة>   | يقوم أمره بتثبيت الحزمة، يمكنك استخدام اسم الحزمة المفضل لديك.|
| npm update <اسم الحزمة>  |سيقوم الأمر  بتحديث الحزمة|
|  npm uninstall <اسم الحزمة>  |سيؤدي هذا الأمر إلى إلغاء تثبيت الحزمة|
|  npm install <اسم الحزمة> -g  |استخدم علامة "-g" لتثبيت حزمة بشكل عام global على جهازك| 
| npm list   |يعدد إصدارات وأسماء جميع الحزم في الدليل الحالي الذي تمت تهيئته| 
| npm i   |يستخدم هذا الأمر ملف package.json كمرجع وسيقوم بتنزيل جميع الحزم المدرجة فيه| 
| npm update  |سيقوم هذا الأمر بتحديث جميع الحزم المثبتة داخل ملف package.json| 
| npm run |استخدم هذا الأمر لتنفيذ الحزم المتاحة للتشغيل| 


## ما هي TypeScript

ال JavaScript هي لغة مفتوحة المصدر وهي مجموعة شاملة من TypeScript
- يقدم ميزات اضافة لجافا سكربت بما في ذالك الانواع الثابتة 
- استخدام الانواع اختياري تماما
- ال  compiles down to regular JS
- يمكن استخدام الواجهة الامامية لـJS بالاضافة الى الواجهة الخلفية مع Node.js
- يتضمن معظم المميزات من ES6 و ES7 (الفئات ووظائف الاسهم وما الى ذالك)
- يمكن اضافة انواع من مكتبات الجهات الخارجية مع تعريفات النوع





## ال Dynamic VS Static Typing

- في اللغات   Dynamic Typed ، ترتبط الأنواع بقيم وقت التشغيل ولا يتم تسميتها صراحة في التعليمات البرمجية الخاصة بك
-  في  اللغات Static Typed ، تقوم بشكل صريح بتعيين أنواع للمتغيرات function parameters , وقيم الارجاع وما الى ذالك
- أمثلة على الديناميك (Java,C,C++,Rust,Go)
- امثلة على الثاتب (JavaScript, Python ,Ruby , PHP)



## ال Compiling TypeScript
- يستخدم TypeScript ملحقات .ts و. tx
- يستخدم TSC (compile   TypeScript) لترجمة ملفات .ts وصولاً إلى JS
- يمكن مشاهدة الملفات والإبلاغ عن الأخطاء في compile time
- تتضمن العديد من الأدوات تجميع TS بشكل افتراضي
- تتمتع معظم IDEs بدعم كبير لـ TS 
- يتم استخدام ملف tsconfig.json لتكوين طريقة عمل TypeScript

## تثبيت وإعداد TypeScript

يتم تثبيت تايب سكريبت عن طريق مدير الحزم NPM كما يلي:

      npm install -g typescript

البارامتر -g يعني بأننا قمنا بتثبيت الحزمة بشكل عام() في جهازنا ومن الممكن استخدامها والوصول إليها من أي مشروع أو مجلد وليس المشروع الحالي فقط.

سنقوم باختبار تايب سكريبت عن طريق الكود أسفله، والذي كما تلاحظون هو مجرد كود جافا سكريبت اعتيادي، ولكنه موجود في ملف امتداده .ts وليس .js.



##### يتم اضافة tsconfig.json  بألامر التالي

     tsc --init
     
```diff
! يجب استخدام tsc  ملحقاتها  في  Command  لتجنب الاخطاء 
```


## أهم مزايا TypeScript

1. دعم الأنواع

- لغات تتحقق من أنواع المتغيرات خلال مرحلة الترجمة أو Compilation، ولذلك يسمى دعمها للأنواع بالدعم الستاتيكي أو الصريح (Static Type Checking). من هذه اللغات نجد جافا، ++C و Go. عندما تصادف هذه اللغات خطأ متعلق بنوع المتغير في الكود فإن الترجمة تفشل ولا تتم بنجاح.

- وصنف آخر من اللغات يقوم بالتحقق من أنواع المتغيرات بشكل ديناميكي (Dynamic Type Checking) أثناء تشغيل البرنامج، ومن هذا الصنف نجد جافا سكريبت، بايثون و PHP.

## الأنواع المدعومة من طرف TypeScript

 بالإضافة لنوع String  تدعم لغة تايب سكريبت عددا من الأنواع الأخرى ونذكر منها أهمها:

#### Boolean

يستخدم هذا النوع للتأكد من أن المتغير هو فعلا Boolean ويقبل إحدى القيمتين true أو false.
  
     let myBool: boolean = false;
     
#### Number

جميع الأعداد الصحيحة (Integers) والعشرية (Decimal) يعتبرها TypeScript من نوع Number، ويضيف إليها كذلك الأعداد من أنظمة Octal ،Hexadecimal و Binary. هذين الأخيرين مدعومين كذلك في جافا سكريبت في الإصدار ES6.

      let intNumber: number = 6;
      let decNumber: number = 6.5;
      let hexNumber: number = 0xf00d;
      let binaryNumber: number = 0b1010;
      let octalNumber: number = 0o744;
      
      
 #### Array
 
 يدعم كذلك تايب سكريبت نوع المصفوفات، ويمكن التصريح بهذا النوع من المتغيرات بطريقتين مختلفتين:
 
 - الطريقة الأولى

        let list: number[] = [1, 2, 3];
         

نلاحظ أننا استعملنا الكلمة number وأمامها معقوفتين [] لكي نخبر تايب سكريبت بأننا أولا نريد مصفوفة وثانيا نريد من هذه المصفوفة أن تحتوي على أعداد فقط.


-الطريقة الثانية

        let list: Array<number> = [1, 2, 3];


#### إذا أردنا مصفوفة عشوائية، بأنواع مختلطة نستعمل النوع any:

        let list: any[] = [1, 'hello', true];

 #### Any
 
 هذا النوع فريد من نوعه مقارنة بالأنواع الأخرى. عن طريقه نرسل رسالة لمترجم تايب سكريبت بأننا غير متأكدين من نوع أو طبيعة المتغير، وأن الأخير قد يكون من أي نوع كان بحسب القيمة المسندة إليه.
 
 يمكن النظر إلى any على أنه الأقرب إلى آلية Dynamic Typing التي تنهجها لغة البرمجة جافا سكريبت نفسها.

      let notSure: any = 5;
      notSure = 'hello world'; // Ok
      notSure = false; // Ok
      
 #### بالإضافة إلى ما ذكرناه، هناك مجموعة من الأنواع الأخرى:

- ال Tuple
- ال Enum
- ال Void
- ال Null and Undefined
- ال Never
- ال Object

تفاصيل وشرح لجميع الأنواع تجدونها على في [ هذا الرابط](https://www.typescriptlang.org/docs/handbook/basic-types.html)

## 2. الدوال في TypeScript

ضيف لغة TypeScript مجموعة من المميزات للدوال، فإلى جانب تحديد نوع البارامترات الذي اكتشفناه أعلاه، يمكننا كذلك تحديد نوع القيمة المرجعة من طرف الدالة

        function greeter(name: string): string {
          return 'Hello, ' + name;
        }

## 3. الواجهات (Interfaces)

تتيح لنا الواجهات تعيين الخصائص والوظائف الواجب توفرها في كائن (Object) أو صنف (Class) محدد.


نقوم بالتصريح بالواجهة في TypeScript بهذه الطريقة:



      interface Person {
        firstName: string;
        lastName: string;
      }
      
ويمكننا استخدامها تماما مثلما نستعمل الأنواع الأساسية المدعومة من لغة البرمجة Typescript.


      function greeter(person: Person) {
        return 'Hello, ' + person.firstName + ' ' + person.lastName;
      }
      
يمكن للكائن person هنا أن يحتوي على خاصيات إضافية ولكن من الضروري أن يتوفر على الأقل على الخاصيتين firstName و lastName المصرح بهما في واجهة Person.

      interface Person {
        firstName: string;
        lastName: string;
        getFullName(): string;
      }
      class Student implements Person {
        constructor(public firstName: string, public lastName: string) {}

        getFullName() {
          return this.firstName + ' ' + this.lastName;
        }
      }

      var student = new Student('Aissa', 'BOUGUERN');

      console.log(student.getFullName()); // Aissa BOUGUERN
      
لاحظوا أننا استعملنا الكلمة implements لنطلب من الصنف Student اتباع بنية الواجهة Person.

#### اضافات VScode 

- TypeScript
- ESLint
- Prettier 
- Error Lens


## الاوامر 

         npm i -g typescript 
         npm i -g nodemon
         npm i -g ts-node
         tsc --init
         tsc -- watch ( file name).ts
         
