# DIAGRAM CATALOG

## Existing diagram files (scan)
- 02_ASSETS/Diagrams/Untitled (2).pdf
- 02_ASSETS/Diagrams/appArt.pdf
- 02_ASSETS/Diagrams/conceptual.pdf
- 02_ASSETS/Diagrams/domain.pdf
- 02_ASSETS/Diagrams/integration&API.pdf
- 02_ASSETS/Diagrams/logical.pdf
- 02_ASSETS/Diagrams/physycal.pdf
- 02_ASSETS/Diagrams/processmodel.pdf
- 02_ASSETS/Diagrams/roadmap.pdf
- 02_ASSETS/Diagrams/security.pdf
- 02_ASSETS/Diagrams/structre & navigation.pdf
- 02_ASSETS/Diagrams/useCase.pdf

| DiagramID | DiagramType | DiagramName | Description | Purpose | OwnerTool | Status | Inputs(files) | Outputs(export filename) | RequiredBy(ReqIDs) | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
|D-001|Conceptual Model|conceptual|نموذج مفاهيمي للكيانات والحدود على مستوى عالي.|تقديم تصور عام للكيانات الأساسية وحدود النطاق.|Miro|EXISTS|03_DATA_MODEL/Data_Dictionary.csv;02_RTM/RTM.csv|02_ASSETS/Diagrams/conceptual.pdf|FR-001;FR-002;FR-003;FR-004;FR-005;FR-006|يوجد ملف PDF.|
|D-002|Domain Model|domain|نموذج علاقات الأعمال بين الكيانات (Business Objects).|توضيح علاقات الأعمال الأساسية بين الكيانات.|Miro|EXISTS|03_DATA_MODEL/Data_Dictionary.csv;02_RTM/RTM.csv|02_ASSETS/Diagrams/domain.pdf|FR-001;FR-002;FR-003;FR-004;FR-005;FR-006;FR-007;FR-008|يوجد ملف PDF.|
|D-003|Logical ERD|logical|مخطط منطقي للجداول والحقول الرئيسية.|توثيق العلاقات المنطقية للبيانات.|SQL Modeler|EXISTS|03_DATA_MODEL/Data_Dictionary.csv|02_ASSETS/Diagrams/logical.pdf|FR-001;FR-002;FR-003;FR-004;FR-005;FR-006;FR-007;FR-008|يوجد ملف PDF.|
|D-004|Physical ERD|physical|مخطط فيزيائي للجداول والقيود والفهارس.|توثيق البنية الفيزيائية للبيانات.|SQL Modeler|EXISTS|03_DATA_MODEL/Data_Dictionary.csv|02_ASSETS/Diagrams/physycal.pdf|FR-001;FR-002;FR-003;FR-004;FR-005;FR-006;FR-007;FR-008|يوجد ملف PDF.|
|D-005|Process Model|process|نموذج عمليات شامل لتدفق العمل الأساسي.|توحيد فهم عمليات المصنع الأساسية.|Miro|EXISTS|02_RTM/RTM.csv;04_UI_PAGES/Pages_Index.csv|02_ASSETS/Diagrams/processmodel.pdf|FR-013;FR-020;FR-039;FR-048;FR-059;UC-001;UC-003;UC-004;UC-005|يوجد ملف PDF.|
|D-006|Use Case Diagram|useCase|مخطط حالات الاستخدام الرئيسية.|عرض تفاعلات المستخدمين مع النظام.|Miro|EXISTS|02_RTM/RTM.csv|02_ASSETS/Diagrams/useCase.pdf|UC-001;UC-002;UC-003;UC-004;UC-005;UC-006;UC-007;UC-008;UC-009;UC-010|يوجد ملف PDF.|
|D-007|App Architecture|appArt|معمارية التطبيق والمكونات والتكاملات.|توضيح مكونات النظام وتدفقات الاتصال.|Miro|EXISTS|05_API/API_Inventory.csv;05_API/Integration_Priority.csv|02_ASSETS/Diagrams/appArt.pdf|FR-076;FR-082;API-001;API-002;API-003;API-004|يوجد ملف PDF.|
|D-008|Integration/API Architecture|integration&API|معمارية التكامل والـ API واتجاهات الاتصال والمصادقة.|توضيح تكاملات الأنظمة والضوابط.|Miro|EXISTS|05_API/API_Inventory.csv;05_API/Integration_Priority.csv|02_ASSETS/Diagrams/integration&API.pdf|FR-076;FR-082;SEC-008;SEC-009;SEC-010|يوجد ملف PDF.|
|D-009|Security Architecture|security|هيكل الأمان (RBAC + RLS + Audit).|توضيح الضوابط والصلاحيات.|Miro|EXISTS|06_SECURITY/RBAC_Matrix.csv;02_RTM/RTM.csv|02_ASSETS/Diagrams/security.pdf|SEC-001;SEC-002;SEC-005;SEC-006;SEC-007|يوجد ملف PDF.|
|D-010|Structure & Navigation|structre & navigation|خريطة هيكلية الصفحات والتنقل.|توضيح بنية الصفحات ومسارات المستخدم.|Miro|EXISTS|04_UI_PAGES/Pages_Index.csv|02_ASSETS/Diagrams/structre & navigation.pdf|P-010;P-020;P-030;P-040;P-045;P-050;P-060;P-070;P-075;P-080;P-090;P-095;P-100;P-110|يوجد ملف PDF.|
|D-011|Roadmap|roadmap|خارطة الطريق الزمنية للإصدارات (MVP/V1.1/V1.2).|توثيق مراحل التطوير.|Miro|EXISTS|99_INTAKE/SRS_TEXT.md|02_ASSETS/Diagrams/roadmap.pdf|FR-091;FR-092;FR-093;FR-094;FR-095;FR-096;FR-097;FR-098|يوجد ملف PDF.|
|D-012|Unknown|Untitled (2)|ملف مخطط غير معنون ولا يمكن تحديد نوعه من الاسم.|يتطلب مراجعة لتحديد الاستخدام.|Miro|EXISTS|02_ASSETS/Diagrams/Untitled (2).pdf|02_ASSETS/Diagrams/Untitled (2).pdf|N/A|OPEN INPUT: تحديد محتوى المخطط من المالك.|
|D-013|Process Flow|Distribution Process|تدفق التوزيع الآلي واليدوي مع التسجيل وUndo وWIP.|توحيد خطوات التوزيع والمسؤوليات.|Miro|CREATE|02_RTM/RTM.csv;04_UI_PAGES/Pages_Index.csv;02_ASSETS/Tables/Stages_List.csv|TBD|FR-013;FR-014;FR-015;FR-016;FR-017;UC-001;UC-002|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-014|Process Flow|Production Logging Process|دخول الموظف وتسجيل بدء/إنهاء مع القيود والتدريب.|توضيح تدفق التسجيل على Mobile/Kiosk.|Miro|CREATE|02_RTM/RTM.csv;04_UI_PAGES/Pages_Index.csv;03_DATA_MODEL/Data_Dictionary.csv|TBD|FR-020;FR-021;FR-022;FR-023;FR-024;FR-025;FR-026;FR-027;FR-029;FR-030;FR-031;UC-003|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-015|Process Flow|QC & Repair Process|تدفق QC والعيوب والتذاكر والإشعارات.|توضيح مسار الجودة والإصلاح.|Miro|CREATE|02_RTM/RTM.csv;02_ASSETS/Tables/Defects_Catalog.csv;02_ASSETS/Tables/Defect_Stage_Map.csv|TBD|FR-039;FR-040;FR-041;FR-042;FR-043;FR-044;FR-045;FR-047;FR-048;FR-049;UC-004;UC-005|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-016|Process Flow|Training Gate Process|تدفق التدريب والاختبار والإقرار قبل التسجيل.|توضيح بوابة التدريب.|Miro|CREATE|02_RTM/RTM.csv;04_UI_PAGES/Pages_Index.csv;02_ASSETS/Tables/WhatsApp_Templates.csv|TBD|FR-036;FR-037;FR-038;UC-006|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-017|Process Flow|Payroll Process|تجميع الإنتاج وNPT والتسعير وتشغيل المسير.|توضيح تدفق الرواتب.|Miro|CREATE|02_RTM/RTM.csv;04_UI_PAGES/Pages_Index.csv;03_DATA_MODEL/Data_Dictionary.csv|TBD|FR-059;FR-060;FR-061;FR-064;UC-007|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-018|Process Flow|Notification Process|تدفق الإشعارات من الحدث حتى التتبع.|توضيح مسار الإشعارات وربط القوالب.|Miro|CREATE|02_RTM/RTM.csv;02_ASSETS/Tables/WhatsApp_Templates.csv;03_DATA_MODEL/Data_Dictionary.csv|TBD|FR-050;FR-051;FR-052;FR-053;FR-054|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-019|Integration Flow|Offline Sync (PWA)|تدفق مزامنة Offline Queue عبر API-004.|توضيح التكامل مع التطبيق دون اتصال.|Miro|CREATE|05_API/API_Inventory.csv;03_DATA_MODEL/Data_Dictionary.csv;02_RTM/RTM.csv|TBD|FR-098;API-004|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-020|Decision/Rule Flow|Spec-to-Stage Rules|قواعد إدراج مراحل الغسيل/التطريز/الإكسسوار.|توثيق منطق توليد المسار.|Miro|CREATE|02_ASSETS/Tables/Spec_to_Stage_Rules.md;02_RTM/RTM.csv|TBD|FR-032;FR-033;FR-034|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-021|Decision/Rule Flow|ETA & Bottleneck Algorithms|منطق ETA والاختناق وفق أداء 7 أيام وWIP.|توثيق خوارزميات التخطيط.|Miro|CREATE|02_RTM/RTM.csv;99_INTAKE/SRS_TEXT.md|TBD|ALG-001;ALG-002;ALG-003;FR-055;FR-056;FR-058|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-022|Security|RBAC & RLS Flows|أدوار وصلاحيات وقيود RLS وإجراءات حساسة.|توضيح التحكم بالوصول.|Miro|CREATE|06_SECURITY/RBAC_Matrix.csv;02_RTM/RTM.csv|TBD|SEC-001;SEC-002;SEC-006;SEC-007|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
|D-023|Architecture|Ops/Deployment Architecture|بيئات النشر والترحيل والنسخ الاحتياطي والمراقبة.|توضيح بنية التشغيل والنشر.|Miro|CREATE|08_OPS/Deployment_Runbook.md|TBD|NFR-010;NFR-011;NFR-005|لا يوجد ملف مطابق في 02_ASSETS/Diagrams.|
