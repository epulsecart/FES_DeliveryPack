# سيناريوهات UAT

كل سيناريو يجب ربطه بـ ReqIDs في RTM.

## Scenario UAT-001
- Preconditions: مسؤول النظام مسجل؛ لا توجد مراحل مُعرّفة مسبقا
- Steps: إنشاء نوع مرحلة ثم إنشاء مرحلة مرتبطة به
- Expected Results: تم الحفظ والمرحلة تظهر في القوائم
- Related ReqIDs: FR-001, FR-002, P-020, P-030

## Scenario UAT-002
- Preconditions: عناصر جاهزة للتوزيع
- Steps: تشغيل التوزيع الآلي ثم اعتماد/تعديل بواسطة أمين المستودع
- Expected Results: يتم ترتيب العناصر حسب القواعد وتُحفظ التعديلات
- Related ReqIDs: FR-013, UC-001, P-050, ALG-003

## Scenario UAT-003
- Preconditions: عنصر غير موزع
- Steps: تنفيذ توزيع يدوي مع سبب ثم تنفيذ Undo بصلاحية مشرف
- Expected Results: تُسجل الأسباب ويُسجل الإلغاء في التدقيق
- Related ReqIDs: FR-014, FR-017, UC-002, SEC-005

## Scenario UAT-004
- Preconditions: موظف مخول بمرحلة ولديه منتج صالح
- Steps: دخول عبر Badge، اختيار مرحلة، مسح رقم المنتج، تسجيل بدء/إنهاء
- Expected Results: يُحفظ سجل الإنتاج وتُحسب المدة
- Related ReqIDs: FR-020, FR-022, FR-024, FR-025, FR-026, FR-027, UC-003, P-060

## Scenario UAT-005
- Preconditions: موظف لم يُكمل التدريب المطلوب
- Steps: محاولة تسجيل إنتاج للمرحلة
- Expected Results: يُمنع التسجيل حتى إكمال التدريب
- Related ReqIDs: FR-037, UC-006, P-045, P-060

## Scenario UAT-006
- Preconditions: منتج يحتاج فحص مخفي
- Steps: إجراء QC مخفي ومطابقة المواصفات/المقاسات
- Expected Results: عند الفشل تُنشأ تذكرة إصلاح إلزامية
- Related ReqIDs: FR-045, UC-004, P-070, P-075

## Scenario UAT-007
- Preconditions: تذكرة إصلاح لها موعد محدد
- Steps: تجاوز موعد الإصلاح ثم محاولة تسجيل إنتاج
- Expected Results: يُمنع التسجيل إلا باستثناء مدير الإنتاج
- Related ReqIDs: FR-048, FR-049, UC-005, SEC-007

## Scenario UAT-008
- Preconditions: بيانات إنتاج لآخر 7 أيام
- Steps: فتح لوحة التخطيط ومراجعة الاختناقات وETA
- Expected Results: تظهر مؤشرات الاختناق وETA محسوب
- Related ReqIDs: FR-055, FR-056, FR-058, ALG-001, ALG-002, P-080

## Scenario UAT-009
- Preconditions: بيانات إنتاج وQC موجودة
- Steps: فتح صفحة التقارير وتصدير تقرير إنتاج وQC
- Expected Results: يتم توليد التقرير وتصديره
- Related ReqIDs: FR-065, FR-071, UC-008, P-110

## Scenario UAT-010
- Preconditions: سجلات إنتاج وأسعار وNPT متاحة
- Steps: تشغيل مسير الرواتب ومراجعة النتائج
- Expected Results: تُحتسب الأجور ويُنتج تقرير الرواتب
- Related ReqIDs: FR-059, FR-061, FR-064, UC-007, P-100

## Scenario UAT-011
- Preconditions: تكامل مفعل مع نظام التفصيل
- Steps: استدعاء GET /items/{thobe_num}/status
- Expected Results: تُعاد حركة المنتج وQC وتذاكر الإصلاح وETA
- Related ReqIDs: API-001, UC-009

## Scenario UAT-012
- Preconditions: نقطة Webhook مهيأة وتوقيع HMAC صحيح
- Steps: إرسال حدث تغيير مرحلة عبر Webhook
- Expected Results: يتم تحديث الحالة وقبول الحدث
- Related ReqIDs: API-002, UC-010
