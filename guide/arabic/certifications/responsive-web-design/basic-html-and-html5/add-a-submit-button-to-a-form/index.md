title: Add a Submit Button to a Form	
localeTitle: undefined
---	## إضافة زر إرسال إلى نموذج

في هذا التحدي ، تريد إدراج زر الإرسال باعتباره آخر عنصر في النموذج (قبل علامة الإغلاق `</form>` ) ولإعطائه `type="submit"` السمة `type="submit"` (كل شيء صغير) ومحتوى نصي من "إرسال "(الحرف الأول من الأحرف الكبيرة) كما هو محدد في إرشادات التحدّي.

1) تكون قيمة `submit` `type` السمة صالحة أيضًا داخل علامة `input` وستعرض زرًا له نفس السلوك تقريبًا ، ولكن هذه ليست العلامة التي تريد استخدامها في هذا التحدي.

 `<input type="submit"> 
` 

إذا لم تحدد قيمة ، فسيحتوي الزر على قيمة افتراضية تم اختيارها من قِبل وكيل المستخدم (عادةً ما يكون هذا بمثابة "إرسال" أو "إرسال الاستعلام").

إذا كنت ترغب في تحديد قيمة مثل "إرسال طلب" ، فيمكنك إجراء ذلك على النحو التالي:

 `<input type="submit" value="Send Request"> 
`