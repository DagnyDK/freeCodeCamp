---
title: ACID
localeTitle: ACID
---
## حامض

في علم الكمبيوتر ، ACID (Atomicity، Consistency، Isolation، Durability) هي مجموعة من الخصائص لتعديلات قاعدة البيانات. فهي تساعد على ضمان صلاحية المعاملة ، حتى مع وجود أخطاء أو إخفاقات.

**المعاملة** هي أي تسلسل من عمليات قاعدة البيانات التي تلبي خصائص ACID ويمكن عرضها كعملية منطقية واحدة على البيانات. مثال على ذلك هو تحويل الأموال من حساب مصرفي إلى حساب آخر. يتضمن هذا عدة تغييرات ، مثل الخصم من حساب واحد واعتماد آخر ، ولكن يعتبر معاملة واحدة.

### Atomicity

وهذا يعني أن المعاملة المعقدة إما يتم معالجتها تمامًا ، أو لا تتم معالجتها على الإطلاق. إذا فشل جزء من المعاملة ، فلن تكتمل المعاملة بالكامل ولن تتغير قاعدة البيانات. بهذه الطريقة ، إذا كان هناك تعطل ، أو عطل في الطاقة ، أو خطأ ، فإن قاعدة البيانات لا ينتهي بها المطاف في حالة حيث يتم تنفيذ أجزاء فقط من المعاملة.

### التناسق

وهذا يعني أن البيانات ستكون متسقة. يجب أن تكون أي بيانات يتم إدخالها في قاعدة البيانات صالحة ومسموح بها وفقًا لأي قيود تحددها. فإنه يتأكد من أن أي معاملة يغير قاعدة البيانات من حالة صالحة واحدة إلى حالة صالحة أخرى.

### عزل

وهذا يعني أنه في حال تنفيذ عمليتين في نفس الوقت ، لا يمكن لمعاملة واحدة قراءة البيانات من معاملة لم تكتمل بعد. سترى كل معاملة قاعدة البيانات كما لو أن المعاملات كانت تنفذ بالتتابع. إذا احتاجت إحدى المعاملات إلى قراءة البيانات التي يكتبها الآخر ، فيجب الانتظار حتى انتهاء المعاملة الأخرى. لن تؤثر تأثير المعاملة غير المكتملة على معاملة أخرى.

### متانة

وهذا يعني أنه بمجرد اكتمال المعاملة ، سيظل الأمر كذلك ، حتى في حالة فقدان الطاقة أو أي أخطاء أخرى. يضمن ذلك تسجيل كافة التغييرات إلى وسيطة تخزين غير متطايرة (مثل القرص الثابت) ، ويقوم بتسجيل سجل المعاملة المكتملة.

### معلومات اكثر:

*   حمض المادة: [ويكيبيديا](https://en.wikipedia.org/wiki/ACID)
*   نظرة عامة على الفيديو: [YouTube](https://www.youtube.com/watch?v=LSB4eceRsw8)