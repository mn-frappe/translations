# Frappe / ERPNext Application Glossary

**Source:** Translation files (`main.pot`) extracted from `/opt/bench/apps/`  
**Languages covered:** English (source)  
**Apps:** frappe · erpnext · hrms · helpdesk · lms · mail  
**Generated:** 2026-05-06

---

## Language File Inventory

| App | Locale directory | Languages available | File format |
|-----|-----------------|--------------------|-|
| **frappe** | `frappe/frappe/locale/` | af ar bs cs da de eo es fa fi fr hr hu id it my nb nl pl pt pt_BR ru sl sr sr_CS sv ta th tr vi zh zh_TW | `.po` / `main.pot` |
| **erpnext** | `erpnext/erpnext/locale/` | af ar bs cs da de eo es fa fi fr hr hu id it my nb nl pl pt pt_BR ru sl sr sr_CS sv ta th tr vi zh zh_TW | `.po` / `main.pot` |
| **hrms** | `hrms/hrms/locale/` | af ar bs cs da de eo es fa fi fr hr hu id it my nb nl pl pt pt_BR ru sl sr sr_CS sv ta th tr vi zh zh_TW | `.po` / `main.pot` |
| **helpdesk** | `helpdesk/helpdesk/locale/` | ar bs cs da de eo es fa fr hr hu id it my nb nl pl pt pt_BR ru sl sr sr_CS sv ta th tr vi zh | `.po` / `main.pot` |
| **lms** | `lms/lms/locale/` | ar bs cs da de eo es fa fr hr hu id it my nb nl pl pt pt_BR ru sl sr sr_CS sv ta th tr vi zh | `.po` / `main.pot` |
| **lms** (legacy) | `lms/lms/translations/` | es | `.csv` |
| **mail** | `mail/mail/locale/` | *(template only, no translations yet)* | `main.pot` |

---

## 1. ERP / Accounting Terms

| Term | Definition | DocType / Module |
|------|-----------|-----------------|
| **Account** | A record in the Chart of Accounts used to classify financial transactions (asset, liability, equity, income, or expense). | Accounts |
| **Asset** | A resource owned by the company that has economic value; tracked for depreciation over its useful life. | Assets |
| **Balance Sheet** | A financial statement showing the company's assets, liabilities, and equity at a specific point in time. | Accounts → Reports |
| **Bank Account** | A ledger account linked to a real-world bank account; used for reconciliation and payment entries. | Accounts |
| **Bank Reconciliation** | The process of matching transactions recorded in ERPNext with the bank statement to identify discrepancies. | Accounts |
| **Budget** | A planned financial target set for a Cost Center or Project for a defined period. | Accounts |
| **Cash Flow** | A report showing the movement of cash in and out of the business during a given period. | Accounts → Reports |
| **Chart of Accounts** | The hierarchical list of all ledger accounts used by the company (assets, liabilities, equity, income, expenses). | Accounts |
| **Cost Center** | An organisational unit used to track expenses and revenues independently (e.g., department, project). | Accounts |
| **Credit** | An entry that increases liability/equity/revenue accounts or decreases asset/expense accounts. | Accounts |
| **Debit** | An entry that increases asset/expense accounts or decreases liability/equity/revenue accounts. | Accounts |
| **Delivery Note** | A document confirming goods dispatched to a customer; reduces stock and is linked to a Sales Order. | Stock |
| **Depreciation** | The systematic allocation of an asset's cost over its useful life, recorded as a periodic expense. | Assets |
| **Expense** | An outflow of money or value incurred in running the business (e.g., salaries, rent, utilities). | Accounts |
| **Fiscal Year** | The 12-month accounting period used for financial reporting; may not coincide with the calendar year. | Accounts |
| **General Ledger** | A complete record of all financial transactions, organised by account; the master report for auditing. | Accounts → Reports |
| **Invoice** | A document requesting payment from a buyer (Sales Invoice) or received from a vendor (Purchase Invoice). | Accounts |
| **Item** | A product or service bought or sold; the central master data used across Stock, Buying, and Selling. | Stock / Setup |
| **Journal Entry** | A manual accounting entry used to record adjustments, accruals, or transactions not covered by standard vouchers. | Accounts |
| **Payable** | Money the company owes to creditors/vendors; recorded as a liability in the Chart of Accounts. | Accounts |
| **Payment** | The act of settling an outstanding invoice; recorded via a Payment Entry in ERPNext. | Accounts |
| **Payment Entry** | A voucher that records the receipt or disbursement of money, and reconciles it against invoices. | Accounts |
| **Profit and Loss** | An income statement showing revenues, costs, and net profit/loss for a defined period. | Accounts → Reports |
| **Purchase Invoice** | A bill received from a supplier; increases Payable and records the expense or stock receipt. | Buying / Accounts |
| **Purchase Order** | A formal document sent to a supplier confirming the intent to buy goods or services at agreed terms. | Buying |
| **Purchase Receipt** | A document confirming receipt of goods from a supplier; increases stock and optionally links to a PO. | Stock / Buying |
| **Quotation** | A formal price offer sent to a prospective customer (also called "Sales Quote"). | Selling |
| **Receipt** | An acknowledgement of money received; in ERPNext often refers to a Payment Entry with the "Receive" mode. | Accounts |
| **Receivable** | Money owed to the company by customers; recorded as an asset in the Chart of Accounts. | Accounts |
| **Revenue** | Income earned from the company's primary business activities (sales of goods or services). | Accounts |
| **Sales Invoice** | A bill issued to a customer for goods or services delivered; increases Receivable. | Selling / Accounts |
| **Sales Order** | A confirmed order from a customer; the basis for invoicing, delivery, and production planning. | Selling |
| **Stock** | Physical inventory of items held in warehouses; tracked by quantity and valuation in ERPNext. | Stock |
| **Tax** | A compulsory financial charge applied to transactions (e.g., VAT, GST, withholding tax). | Accounts / Tax |
| **Trial Balance** | A report listing all ledger account balances to verify that total debits equal total credits. | Accounts → Reports |
| **Voucher** | A generic term for any accounting document (Journal Entry, Payment Entry, etc.) that affects the ledger. | Accounts |
| **Warehouse** | A physical or virtual location where stock items are stored; used for inventory tracking and valuation. | Stock |

---

## 2. HR / Payroll Terms

| Term | Definition | DocType / Module |
|------|-----------|-----------------|
| **Appraisal** | A formal performance evaluation of an employee against predefined goals or KPIs for a review period. | HRMS → Performance |
| **Attendance** | A daily record of whether an employee was present, absent, on leave, or on a half-day for a given date. | HRMS → Attendance |
| **Attendance Request** | A request submitted by an employee to regularise attendance that was not automatically captured. | HRMS → Attendance |
| **Deduction** | An amount subtracted from an employee's gross salary (e.g., income tax, provident fund, loan repayment). | HRMS → Payroll |
| **Gratuity** | A statutory end-of-service benefit paid to an employee upon resignation or termination after a minimum tenure. | HRMS → Payroll |
| **Interview** | A structured evaluation session in the recruitment process used to assess a candidate's suitability. | HRMS → Recruitment |
| **Job Offer** | A formal document extended to a selected candidate confirming the terms of employment. | HRMS → Recruitment |
| **Job Opening** | A vacancy posted internally or publicly to attract candidates for a specific role. | HRMS → Recruitment |
| **Leave** | Authorised absence from work; categorised by type (annual, sick, casual, etc.) and tracked against a balance. | HRMS → Leave |
| **Leave Application** | A formal request submitted by an employee to take leave for specified dates. | HRMS → Leave |
| **Onboarding** | The structured process of integrating a new hire into the company, including document collection and orientation tasks. | HRMS → Employee Lifecycle |
| **Overtime** | Additional hours worked beyond the regular shift, often compensated at a premium pay rate. | HRMS → Attendance |
| **Payroll** | The process of calculating and disbursing employee salaries, including earnings, deductions, and tax; results in Salary Slips. | HRMS → Payroll |
| **Recruitment** | The end-to-end process of sourcing, evaluating, and hiring candidates for open positions. | HRMS → Recruitment |
| **Salary Slip** | A per-employee document generated during the payroll run detailing gross pay, deductions, and net pay. | HRMS → Payroll |
| **Training** | Organised learning activities (programs or events) assigned to employees to develop skills. | HRMS → Training |

---

## 3. Helpdesk / Support Terms

| Term | Definition | DocType / Module |
|------|-----------|-----------------|
| **Agent** | A support team member who handles and resolves customer tickets in Frappe Helpdesk. | Helpdesk |
| **Article** | A help-centre document published in the Knowledge Base to enable customer self-service. | Helpdesk → Knowledge Base |
| **Category** | A classification label applied to tickets or articles to aid routing, reporting, and filtering. | Helpdesk |
| **Contact** | A person associated with a customer account; may be the reporter of a support ticket. | Helpdesk / CRM |
| **Customer** | A company or individual that has a support relationship and can raise tickets. | Helpdesk |
| **Feedback** | A customer's post-resolution rating or comment on the quality of support received. | Helpdesk |
| **Knowledge Base** | A repository of articles and FAQs that agents and customers can search for self-service resolution. | Helpdesk |
| **Priority** | The urgency level assigned to a ticket (e.g., Low, Medium, High, Urgent) that influences SLA deadlines. | Helpdesk |
| **Rating** | A numeric or star-based score given by a customer to evaluate the support experience. | Helpdesk |
| **Resolution** | The action or explanation that closes a ticket; the final answer to a customer's issue. | Helpdesk |
| **SLA** | *Service Level Agreement* — a policy defining the maximum response and resolution times for tickets based on priority. | Helpdesk |
| **Status** | The current state of a ticket in its lifecycle (e.g., Open, Replied, Resolved, Closed). | Helpdesk |
| **Team** | A group of agents organised by function or product area; tickets can be assigned to a team. | Helpdesk |
| **Ticket** | The core support record capturing a customer's request, question, or complaint, from creation to closure. | Helpdesk |

---

## 4. LMS / Learning Terms

| Term | Definition | DocType / Module |
|------|-----------|-----------------|
| **Assignment** | A task given to students within a lesson or course that requires submission and optional review. | LMS |
| **Batch** | A cohort of students enrolled in a course for a specific time period; enables group management. | LMS |
| **Certificate** | A digital credential issued to a student upon successful completion of a course or program. | LMS |
| **Certification** | The formal process of awarding a certificate; may involve passing a quiz or meeting a minimum score. | LMS |
| **Chapter** | A logical grouping of lessons within a course, used to organise content into thematic sections. | LMS |
| **Course** | The primary learning unit containing chapters, lessons, quizzes, and assignments on a specific topic. | LMS |
| **Evaluation** | An assessment activity used to measure student understanding; may be a quiz, assignment, or project. | LMS |
| **Instructor** | A user who creates and delivers course content; can host live classes and review assignments. | LMS |
| **Lesson** | The smallest content unit within a course chapter; contains video, text, or interactive material. | LMS |
| **Live Class** | A scheduled real-time session (e.g., video call) conducted by an instructor for enrolled students. | LMS |
| **Program** | A structured collection of multiple courses grouped into a curriculum or learning path. | LMS |
| **Progress** | The percentage of course content a student has completed, tracked per lesson or chapter. | LMS |
| **Quiz** | A set of questions presented to a student to test knowledge; results can determine course completion. | LMS |
| **Student** | A user enrolled in one or more courses; their progress, quiz scores, and certificates are tracked. | LMS |

---

## 5. Mail / Communication Terms

| Term | Definition | DocType / Module |
|------|-----------|-----------------|
| **Alias** | An alternative email address that forwards or delivers messages to a primary mailbox. | Mail |
| **DKIM** | *DomainKeys Identified Mail* — a cryptographic email-authentication method that attaches a digital signature to outgoing mail, allowing receivers to verify the sender's domain. | Mail / DNS |
| **DMARC** | *Domain-based Message Authentication, Reporting & Conformance* — a policy that instructs receiving mail servers how to handle messages that fail SPF or DKIM checks. | Mail / DNS |
| **Domain** | The registered internet domain (e.g., `example.com`) used for sending and receiving email. | Mail |
| **Mailbox** | A dedicated inbox associated with a specific email address on the mail server. | Mail |
| **Newsletter** | A bulk email message sent to a list of subscribers; tracked for delivery and open rates. | Mail |
| **Queue** | The ordered list of outgoing email messages waiting to be delivered by the mail server. | Mail |
| **Signature** | A block of text or HTML appended automatically to outgoing emails (e.g., name, title, contact details). | Mail |
| **SPF** | *Sender Policy Framework* — a DNS record that specifies which mail servers are authorised to send email on behalf of a domain; helps prevent spoofing. | Mail / DNS |
| **Thread** | A chain of related email messages (original message + all replies) grouped together for context. | Mail |

---

## 6. Manufacturing / BOM Terms

| Term | Definition | DocType / Module |
|------|-----------|-----------------|
| **BOM (Bill of Materials)** | A structured list of all raw materials, sub-assemblies, components, and quantities required to manufacture one unit of a finished product. The central document driving production planning and cost calculation. | Manufacturing |
| **Batch** | A group of units produced or received together and assigned a shared identifier for traceability, expiry tracking, and quality control. | Stock / Manufacturing |
| **Finished Good** | An item that has completed the manufacturing process and is ready for sale or distribution. | Manufacturing / Stock |
| **Job Card** | A work-order-level instruction document issued to a specific workstation, detailing the operation to perform, the time allocated, and materials consumed. | Manufacturing |
| **Manufacture** | The process of producing a finished good from raw materials by executing a Work Order against a BOM. | Manufacturing |
| **Packing Slip** | A document listing the contents of a shipment, attached to a delivery to help the receiver verify the items packed. | Stock |
| **Process Loss** | The expected or actual quantity of material lost during a manufacturing operation (e.g., evaporation, offcuts, waste). | Manufacturing |
| **Production Plan** | A planning document that consolidates sales orders and material requests to schedule Work Orders and purchase requirements for a given period. | Manufacturing |
| **Quality Inspection** | A formal check performed on incoming, in-process, or outgoing items to verify they meet defined acceptance criteria. | Quality / Stock |
| **Raw Material** | An unprocessed or minimally processed input item consumed during manufacturing to produce a finished or semi-finished good. | Manufacturing / Stock |
| **Routing** | An ordered sequence of operations (each tied to a Workstation) that defines the manufacturing path for a BOM. | Manufacturing |
| **Scrap** | Material that is discarded or by-produced during a manufacturing process; may have a residual value that affects production cost. | Manufacturing |
| **Serial No** | A unique identifier assigned to an individual unit of an item for full traceability throughout its lifecycle (purchase → sale → warranty). | Stock |
| **Subcontracting** | A manufacturing arrangement where certain operations or assemblies are outsourced to a third-party vendor, who receives raw materials and returns finished goods. | Manufacturing / Buying |
| **Work Order** | A production instruction document that authorises the manufacture of a specific quantity of an item against a BOM, tracks material consumption, and records actual vs. planned time. | Manufacturing |
| **Workstation** | A physical or logical production location (machine, bench, line) where a specific manufacturing operation is performed; used for capacity and cost planning. | Manufacturing |

---

*This glossary was auto-generated from `main.pot` translation template files. Definitions reflect the usage context within the Frappe framework and its applications.*

---

# Frappe / ERPNext Нэр томьёоны тайлбар толь (Монгол)

**Эх сурвалж:** `/opt/bench/apps/` дахь орчуулгын файлуудаас гаргасан  
**Хэл:** Монгол  
**Аппууд:** frappe · erpnext · hrms · helpdesk · lms · mail  

---

## 1. ERP / Нягтлан бодох бүртгэлийн нэр томьёо

| Нэр томьёо (EN) | Монгол нэршил | Тайлбар | Модуль |
|----------------|--------------|---------|--------|
| **Account** | **Данс** | Санхүүгийн гүйлгээг ангилахад ашигладаг дансны дэвтэр дэх бичилт (хөрөнгө, өр төлбөр, өмч, орлого, зардал). | Нягтлан бодох бүртгэл |
| **Asset** | **Хөрөнгө** | Компанийн эзэмшдэг, эдийн засгийн үнэ цэнэтэй нөөц; элэгдлийг ашиглалтын хугацаанд хянадаг. | Хөрөнгийн бүртгэл |
| **Balance Sheet** | **Баланс** | Тодорхой өдрийн байдлаар компанийн хөрөнгө, өр төлбөр, өмчийг харуулсан санхүүгийн тайлан. | Тайлан |
| **Bank Account** | **Банкны данс** | Бодит банкны дансанд холбосон дансны дэвтрийн бичилт; нэгтгэл болон төлбөрийн бичилтэд ашиглагдана. | Нягтлан бодох бүртгэл |
| **Bank Reconciliation** | **Банкны нэгтгэл** | ERPNext-д бүртгэсэн гүйлгээг банкны хуулгатай тулгах, зөрүүг илрүүлэх үйл явц. | Нягтлан бодох бүртгэл |
| **Budget** | **Төсөв** | Тодорхой хугацаанд зардлын төвийн эсвэл төслийн хувьд тогтоосон санхүүгийн зорилтот хэмжээ. | Нягтлан бодох бүртгэл |
| **Cash Flow** | **Мөнгөн урсгал** | Тодорхой хугацаанд бизнест орж гарсан мөнгөний хөдөлгөөнийг харуулсан тайлан. | Тайлан |
| **Chart of Accounts** | **Дансны ерөнхий дэвтэр** | Компанийн ашигладаг бүх дансны шаталсан жагсаалт (хөрөнгө, өр төлбөр, өмч, орлого, зардал). | Нягтлан бодох бүртгэл |
| **Cost Center** | **Зардлын төв** | Зардал, орлогыг бие даан хянах зохион байгуулалтын нэгж (жишээ нь, хэлтэс, төсөл). | Нягтлан бодох бүртгэл |
| **Credit** | **Кредит (зээл бичилт)** | Өр төлбөр/өмч/орлогын дансыг нэмэгдүүлэх, эсвэл хөрөнгө/зардлын дансыг бууруулах бичилт. | Нягтлан бодох бүртгэл |
| **Debit** | **Дебит** | Хөрөнгө/зардлын дансыг нэмэгдүүлэх, эсвэл өр төлбөр/өмч/орлогын дансыг бууруулах бичилт. | Нягтлан бодох бүртгэл |
| **Delivery Note** | **Хүргэлтийн баримт** | Худалдан авагчид бараа тушаасан гэдгийг баталгаажуулах баримт бичиг; нөөцийг бууруулж, борлуулалтын захиалгатай холбогдоно. | Нөөц |
| **Depreciation** | **Элэгдэл** | Хөрөнгийн өртгийг ашиглалтын хугацаанд тогтмол зардал болгон хуваарилах үйл явц. | Хөрөнгийн бүртгэл |
| **Expense** | **Зардал** | Бизнес эрхлэхэд гарах мөнгөн гарц (цалин, түрээс, аж ахуйн зардал гэх мэт). | Нягтлан бодох бүртгэл |
| **Fiscal Year** | **Санхүүгийн жил** | Санхүүгийн тайлагналд ашигладаг 12 сарын тооцооны хугацаа; хуанлийн жилтэй давхцахгүй байж болно. | Нягтлан бодох бүртгэл |
| **General Ledger** | **Ерөнхий дэвтэр** | Дансаар ангилсан бүх санхүүгийн гүйлгээний бүрэн бүртгэл; аудитын үндсэн тайлан. | Тайлан |
| **Invoice** | **Нэхэмжлэх** | Худалдан авагчаас (борлуулалтын нэхэмжлэх) эсвэл нийлүүлэгчид (худалдан авалтын нэхэмжлэх) илгээсэн төлбөрийн баримт. | Нягтлан бодох бүртгэл |
| **Item** | **Бараа/Үйлчилгээ** | Худалдан авах эсвэл зарах бараа, үйлчилгээ; нөөц, худалдан авалт, борлуулалтын үндсэн мастер өгөгдөл. | Нөөц / Тохиргоо |
| **Journal Entry** | **Журналын бичилт** | Стандарт баримтаар хамрагдаагүй залруулга, хуримтлал, гүйлгээг бүртгэхэд ашигладаг гараар оруулах нягтлан бодох бүртгэлийн бичилт. | Нягтлан бодох бүртгэл |
| **Payable** | **Өглөг** | Компанийн зээлдүүлэгч/нийлүүлэгчдэд өгөх ёстой мөнгө; дансны дэвтэрт өр төлбөр болгон бүртгэнэ. | Нягтлан бодох бүртгэл |
| **Payment** | **Төлбөр** | Хугацаа хэтэрсэн нэхэмжлэхийг тооцоо нийлэн барагдуулах үйлдэл; ERPNext-д Төлбөрийн бичилт болгон бүртгэнэ. | Нягтлан бодох бүртгэл |
| **Payment Entry** | **Төлбөрийн бичилт** | Мөнгө хүлээн авсан, эсвэл гаргасан баримтыг бүртгэж, нэхэмжлэхтэй нэгтгэдэг баримт бичиг. | Нягтлан бодох бүртгэл |
| **Profit and Loss** | **Ашиг, алдагдлын тайлан** | Тодорхой хугацааны орлого, зардал, цэвэр ашиг/алдагдлыг харуулсан санхүүгийн тайлан. | Тайлан |
| **Purchase Invoice** | **Худалдан авалтын нэхэмжлэх** | Нийлүүлэгчээс ирсэн нэхэмжлэх; өглөгийг нэмэгдүүлж, зардал эсвэл нөөцийн хүлээн авалтыг бүртгэнэ. | Худалдан авалт / Нягтлан бодох бүртгэл |
| **Purchase Order** | **Худалдан авалтын захиалга** | Нийлүүлэгчид тохиролцсон нөхцөлөөр бараа, үйлчилгээ худалдан авах санаа зорилгоо баталгаажуулан илгээдэг албан баримт. | Худалдан авалт |
| **Purchase Receipt** | **Худалдан авалтын хүлээн авалт** | Нийлүүлэгчээс бараа хүлээн авсныг баталгаажуулах баримт; нөөцийг нэмэгдүүлж, захиалгатай холбогдоно. | Нөөц / Худалдан авалт |
| **Quotation** | **Үнийн санал** | Болзошгүй худалдан авагчид илгээх албан ёсны үнийн санал (мөн "Борлуулалтын үнийн санал" гэж нэрлэнэ). | Борлуулалт |
| **Receipt** | **Баримт / Авлага** | Мөнгө хүлээн авсан гэдгийн баталгаа; ERPNext-д ихэвчлэн "Хүлээн авах" горимтой Төлбөрийн бичилтийг хэлнэ. | Нягтлан бодох бүртгэл |
| **Receivable** | **Авлага** | Харилцагчдаас компанид авах мөнгө; дансны дэвтэрт хөрөнгө болгон бүртгэнэ. | Нягтлан бодох бүртгэл |
| **Revenue** | **Орлого** | Компанийн үндсэн үйл ажиллагаанаас (бараа, үйлчилгээ борлуулалт) олж буй орлого. | Нягтлан бодох бүртгэл |
| **Sales Invoice** | **Борлуулалтын нэхэмжлэх** | Хүргэсэн бараа, үйлчилгээний төлөөд харилцагчид олгох нэхэмжлэх; авлагыг нэмэгдүүлнэ. | Борлуулалт / Нягтлан бодох бүртгэл |
| **Sales Order** | **Борлуулалтын захиалга** | Харилцагчаас баталгаажсан захиалга; нэхэмжлэх, хүргэлт, үйлдвэрлэлийн төлөвлөлтийн үндэс. | Борлуулалт |
| **Stock** | **Нөөц / Агуулах** | Агуулахад хадгалагдаж буй барааны физик нөөц; тоо хэмжээ, үнэлгээгээр ERPNext-д хянагдана. | Нөөц |
| **Tax** | **Татвар** | Гүйлгээнд ногдуулдаг заавал төлөх санхүүгийн хуримтлал (НӨАТ, ХААН, суутган татвар гэх мэт). | Нягтлан бодох бүртгэл / Татвар |
| **Trial Balance** | **Туршилтын баланс** | Нийт дебит, кредит тэнцэж байгааг шалгах зорилгоор бүх дансны үлдэгдлийг жагсаасан тайлан. | Тайлан |
| **Voucher** | **Баримт бичиг** | Дансны дэвтэрт нөлөөлдөг дурын нягтлан бодох бүртгэлийн баримт бичгийн нийтлэг нэршил (Журналын бичилт, Төлбөрийн бичилт гэх мэт). | Нягтлан бодох бүртгэл |
| **Warehouse** | **Агуулах** | Нөөцийн барааг хадгалах физик эсвэл виртуал байршил; нөөцийн хяналт, үнэлгээнд ашиглагдана. | Нөөц |

---

## 2. ХН / Цалин хөлсний нэр томьёо

| Нэр томьёо (EN) | Монгол нэршил | Тайлбар | Модуль |
|----------------|--------------|---------|--------|
| **Appraisal** | **Ажлын үнэлгээ** | Тогтоосон зорилт, KPI-ын дагуу ажилтны гүйцэтгэлийг тодорхой хугацаанд албан ёсоор үнэлэх үйл явц. | HRMS → Гүйцэтгэл |
| **Attendance** | **Ирц** | Ажилтан тухайн өдөр ирсэн, тасалсан, чөлөөтэй, хагас өдөр байгааг бүртгэсэн өдрийн бичилт. | HRMS → Ирц |
| **Attendance Request** | **Ирцийн хүсэлт** | Автоматаар бүртгэгдээгүй ирцийг тохируулах зорилгоор ажилтнаас гаргасан хүсэлт. | HRMS → Ирц |
| **Deduction** | **Суутгал** | Ажилтны нийт цалингаас хасах дүн (орлогын татвар, тэтгэврийн шимтгэл, зээлийн эргэн төлөлт гэх мэт). | HRMS → Цалин |
| **Gratuity** | **Ажиллах хугацааны тэтгэмж** | Ажилтан тодорхой хугацаа ажилласны дараа ажлаас гарах эсвэл халагдах үед олгох хуулиар заасан тэтгэмж. | HRMS → Цалин |
| **Interview** | **Ярилцлага** | Нэр дэвшигчийн тохиромжтой байдлыг үнэлэхэд ашигладаг ажилд авах үйл явц дахь бүтэцтэй үнэлгээний хуралдаан. | HRMS → Ажилд авалт |
| **Job Offer** | **Ажлын санал** | Сонгосон нэр дэвшигчид ажил эрхлэлтийн нөхцөлийг баталгаажуулан өгдөг албан баримт бичиг. | HRMS → Ажилд авалт |
| **Job Opening** | **Ажлын байрны зар** | Тодорхой албан тушаалын нэр дэвшигч татах зорилгоор дотооддоо эсвэл нийтэд зарласан ажлын байрны сул орон тоо. | HRMS → Ажилд авалт |
| **Leave** | **Чөлөө** | Ажлаас зөвшөөрлийн дагуу завсарлах; төрлөөр (жилийн, өвчний, ердийн гэх мэт) ангилж, үлдэгдлийг хянана. | HRMS → Чөлөо |
| **Leave Application** | **Чөлөөний өргөдөл** | Ажилтнаас тодорхой өдрүүдэд чөлөо авахыг хүссэн албан хүсэлт. | HRMS → Чөлөо |
| **Onboarding** | **Ажилд орох үйл явц** | Шинэ ажилтныг компанид нэгтгэх бүтэцтэй үйл явц; баримт бичиг цуглуулах болон чиг баримжаа олгох даалгавруудыг агуулна. | HRMS → Ажилтны амьдралын мөчлөг |
| **Overtime** | **Илүү цагийн ажил** | Ердийн ээлжээс гадуур ажилласан нэмэлт цаг; ихэвчлэн нэмэгдүүлсэн цалингаар нөхөн олгоно. | HRMS → Ирц |
| **Payroll** | **Цалин хөлс** | Ажилтны цалин хөлсийг орлого, суутгал, татварыг оруулан тооцоолж, олгох үйл явц; Цалингийн хуудас үүснэ. | HRMS → Цалин |
| **Recruitment** | **Ажилд авалт** | Нэр дэвшигчдийг хайх, үнэлэх, ажилд авах бүхий л үйл явц. | HRMS → Ажилд авалт |
| **Salary Slip** | **Цалингийн хуудас** | Нийт цалин, суутгал, цэвэр цалинг дэлгэрэнгүй харуулсан, цалин тооцооны явцад үүсгэсэн ажилтан бүрийн баримт. | HRMS → Цалин |
| **Training** | **Сургалт** | Ажилтнуудад ур чадвар хөгжүүлэх зорилгоор зохион байгуулдаг сургалтын үйл ажиллагаа (хөтөлбөр, арга хэмжээ). | HRMS → Сургалт |

---

## 3. Тусламжийн ширээ / Дэмжлэгийн нэр томьёо

| Нэр томьёо (EN) | Монгол нэршил | Тайлбар | Модуль |
|----------------|--------------|---------|--------|
| **Agent** | **Оператор** | Frappe Helpdesk-д харилцагчийн тасалбаруудыг хүлээн авч, шийдвэрлэдэг дэмжлэгийн багийн гишүүн. | Helpdesk |
| **Article** | **Нийтлэл** | Харилцагч өөрийн асуудлаа шийдвэрлэх боломж олгох зорилгоор Мэдлэгийн санд нийтлэсэн тусламжийн баримт. | Helpdesk → Мэдлэгийн сан |
| **Category** | **Ангилал** | Тасалбар эсвэл нийтлэлд хэрэглэдэг ангиллын шошго; чиглүүлэлт, тайлагнал, шүүлтэнд туслана. | Helpdesk |
| **Contact** | **Холбогч хүн** | Харилцагчийн дансанд холбоотой хүн; дэмжлэгийн тасалбар гаргасан хүн байж болно. | Helpdesk / CRM |
| **Customer** | **Харилцагч** | Дэмжлэгийн харилцаатай байж, тасалбар үүсгэх боломжтой компани эсвэл хувь хүн. | Helpdesk |
| **Feedback** | **Санал хүсэлт** | Харилцагчийн шийдвэрлэсний дараах үнэлгээ эсвэл хүлээн авсан дэмжлэгийн чанарт хийсэн сэтгэгдэл. | Helpdesk |
| **Knowledge Base** | **Мэдлэгийн сан** | Оператор болон харилцагч өөрийн асуудлаа шийдвэрлэхийн тулд хайж болох нийтлэл, ТУА-ийн агуулах. | Helpdesk |
| **Priority** | **Эрэмбэлэл** | Тасалбарт оноосон яаралтын түвшин (жишээ нь, Бага, Дунд, Өндөр, Яаралтай); SLA-ийн хугацаанд нөлөөлнэ. | Helpdesk |
| **Rating** | **Үнэлгээ** | Харилцагчаас дэмжлэгийн туршлагыг үнэлэхэд өгдөг тоон эсвэл одны оноо. | Helpdesk |
| **Resolution** | **Шийдвэрлэлт** | Тасалбарыг хаах арга хэмжээ эсвэл тайлбар; харилцагчийн асуудалд өгсөн эцсийн хариулт. | Helpdesk |
| **SLA** | **Үйлчилгээний түвшний гэрээ** | Тасалбарын эрэмбэлэлд тулгуурлан хариу болон шийдвэрлэлтийн дээд хугацааг тодорхойлсон бодлого. | Helpdesk |
| **Status** | **Төлөв** | Тасалбарын амьдралын мөчлөг дэх одоогийн байдал (Нээлттэй, Хариулсан, Шийдвэрлэсэн, Хаасан гэх мэт). | Helpdesk |
| **Team** | **Баг** | Чиг үүрэг эсвэл бүтээгдэхүүний чиглэлээр зохион байгуулагдсан операторуудын бүлэг; тасалбарыг багт оноож болно. | Helpdesk |
| **Ticket** | **Тасалбар** | Харилцагчийн хүсэлт, асуулт, гомдлыг үүсгэснээс хаах хүртэл бүртгэдэг дэмжлэгийн үндсэн бичилт. | Helpdesk |

---

## 4. СУС / Сургалтын нэр томьёо

| Нэр томьёо (EN) | Монгол нэршил | Тайлбар | Модуль |
|----------------|--------------|---------|--------|
| **Assignment** | **Даалгавар** | Хичээл эсвэл курс дотор оюутанд өгсөн, илгээж, нэмэлтээр шалгах шаардлагатай ажил. | LMS |
| **Batch** | **Бүлэг** | Тодорхой хугацаанд курст бүртгэлтэй оюутнуудын дэд бүлэг; бүлгийн удирдлагыг хялбарчилна. | LMS |
| **Certificate** | **Гэрчилгээ** | Курс эсвэл хөтөлбөрийг амжилттай дүүргэсний дараа оюутанд олгох цахим баримт бичиг. | LMS |
| **Certification** | **Гэрчилгээжүүлэлт** | Гэрчилгээ олгох албан ёсны үйл явц; шалгалт өгөх эсвэл дахин оноо авсан байх шаардлагатай байж болно. | LMS |
| **Chapter** | **Бүлэг (сэдэв)** | Курс доторх хичээлүүдийн логик бүлэглэл; агуулгыг сэдэвчилсэн хэсгүүдэд зохион байгуулна. | LMS |
| **Course** | **Курс** | Тодорхой сэдвийн дагуу бүлэг, хичээл, шалгалт, даалгаваруудыг агуулсан үндсэн сургалтын нэгж. | LMS |
| **Evaluation** | **Үнэлгээ** | Оюутны ойлголтыг хэмжихэд ашигладаг үнэлгээний үйл ажиллагаа; шалгалт, даалгавар, эсвэл төсөл байж болно. | LMS |
| **Instructor** | **Багш / Зааварлагч** | Курсийн агуулга үүсгэж, хүргэдэг хэрэглэгч; шууд хичээл явуулж, даалгавар шалгаж болно. | LMS |
| **Lesson** | **Хичээл** | Курсийн бүлэг доторх хамгийн жижиг агуулгын нэгж; видео, текст, эсвэл интерактив материал агуулна. | LMS |
| **Live Class** | **Шууд хичээл** | Бүртгэлтэй оюутнуудад зориулан багш хийдэг товлосон бодит цагийн хуралдаан (жишээ нь, видео дуудлага). | LMS |
| **Program** | **Хөтөлбөр** | Сургалтын төлөвлөгөө дотор нэгтгэсэн олон курсын бүтэцтэй цуглуулга. | LMS |
| **Progress** | **Явц** | Оюутны хичээл эсвэл бүлгээр хянагдах дүүргэсэн курсийн агуулгын хувь. | LMS |
| **Quiz** | **Шалгалт / Тест** | Мэдлэгийг шалгах зорилгоор оюутанд үзүүлдэг асуултуудын цуглуулга; үр дүн нь курс дүүргэлтийг тодорхойлж болно. | LMS |
| **Student** | **Оюутан** | Нэг буюу хэд хэдэн курст бүртгэлтэй хэрэглэгч; явц, шалгалтын оноо, гэрчилгээг нь хянана. | LMS |

---

## 5. Шуудан / Харилцааны нэр томьёо

| Нэр томьёо (EN) | Монгол нэршил | Тайлбар | Модуль |
|----------------|--------------|---------|--------|
| **Alias** | **Нэр төрөл / Өөр нэр** | Үндсэн шуудангийн хайрцагт мессежийг дамжуулах эсвэл хүргэх өөр цахим шуудангийн хаяг. | Шуудан |
| **DKIM** | **DKIM (Домайн түлхүүрээр баталгаажуулсан шуудан)** | Гарч буй шуудан дээр цифр гарын үсэг хавсаргадаг криптографийн шуудангийн баталгаажуулалтын арга; хүлээн авагч илгээгчийн домайнийг шалгах боломжийг олгоно. | Шуудан / DNS |
| **DMARC** | **DMARC (Домайнд суурилсан мессежийн баталгаажуулалт)** | SPF эсвэл DKIM шалгалтад тэнцэхгүй мессежийг хүлээн авагч шуудангийн сервер хэрхэн зохицуулах талаарх бодлого. | Шуудан / DNS |
| **Domain** | **Домайн** | Цахим шуудан илгээх, хүлээн авахад ашигладаг бүртгэлтэй интернетийн домайн (жишээ нь, `example.com`). | Шуудан |
| **Mailbox** | **Шуудангийн хайрцаг** | Шуудангийн серверийн тодорхой цахим шуудангийн хаяганд холбоотой тусгай ирэх хавтас. | Шуудан |
| **Newsletter** | **Мэдээллийн товхимол** | Бүртгэлтэй хэрэглэгчдэд хүргэх бөөнөөр илгээдэг цахим шуудангийн мессеж; хүргэлт, нээлтийн тоог хянана. | Шуудан |
| **Queue** | **Дараалал** | Шуудангийн серверээс хүргэхийг хүлээж буй гарах цахим шуудангийн дарааллын жагсаалт. | Шуудан |
| **Signature** | **Гарын үсэг / Хавсралт текст** | Гарч буй цахим шуудан дээр автоматаар нэмэгддэг текст эсвэл HTML блок (жишээ нь, нэр, албан тушаал, холбоо барих мэдээлэл). | Шуудан |
| **SPF** | **SPF (Илгээгчийн бодлогын хүрээ)** | Домайны өмнөөс цахим шуудан илгээх эрхтэй шуудангийн серверүүдийг тодорхойлдог DNS бичилт; хуурамч илгээлтээс хамгаалахад тусалдаг. | Шуудан / DNS |
| **Thread** | **Хэлхээ** | Нэг сэдвээр холбогдсон цахим шуудангийн мессежүүдийн гинж (анхны мессеж + бүх хариулт) нэг дор бүлэглэгдсэн. | Шуудан |

---

## 6. Үйлдвэрлэл / BOM-ийн нэр томьёо

| Нэр томьёо (EN) | Монгол нэршил | Тайлбар | Модуль |
|----------------|--------------|---------|--------|
| **BOM (Bill of Materials)** | **Материалын жагсаалт** | Дуусгавар бүтээгдэхүүний нэг нэгжийг үйлдвэрлэхэд шаардлагатай бүх түүхий эд, угсралт, бүрэлдэхүүн хэсэг, тоо хэмжээний бүтэцтэй жагсаалт. Үйлдвэрлэлийн төлөвлөлт, өртгийн тооцооллын үндсэн баримт. | Үйлдвэрлэл |
| **Batch** | **Багц** | Нэг дор үйлдвэрлэсэн эсвэл хүлээн авсан, мөшгих чадвар, дуусгавар хугацаа, чанарын хяналтын зорилгоор нийтлэг ID оноосон нэгжүүдийн бүлэг. | Нөөц / Үйлдвэрлэл |
| **Finished Good** | **Дуусгавар бүтээгдэхүүн** | Үйлдвэрлэлийн үйл явцыг дүүргэж, борлуулалт, хуваарилалтад бэлэн болсон бараа. | Үйлдвэрлэл / Нөөц |
| **Job Card** | **Ажлын карт** | Гүйцэтгэх үйл ажиллагаа, хуваарилагдсан хугацаа, хэрэглэсэн материалыг дэлгэрэнгүй заасан, тодорхой ажлын байранд олгосон ажлын захиалгын түвшний заавар баримт. | Үйлдвэрлэл |
| **Manufacture** | **Үйлдвэрлэл** | BOM-тай холбоотой Ажлын захиалгыг гүйцэтгэн түүхий эдээс дуусгавар бүтээгдэхүүн үйлдвэрлэх үйл явц. | Үйлдвэрлэл |
| **Packing Slip** | **Савлагааны баримт** | Илгээмжид хавсаргасан, хүлээн авагч нь савласан барааг шалгах боломжтой тээвэрлэлтийн агуулгыг жагсаасан баримт. | Нөөц |
| **Process Loss** | **Үйл явцын алдагдал** | Үйлдвэрлэлийн явцад алдагдах хүлээгдэж буй буюу бодит тоо хэмжээ (жишээ нь, ууршилт, хаягдал хэрчмэл, хог). | Үйлдвэрлэл |
| **Production Plan** | **Үйлдвэрлэлийн төлөвлөгөө** | Борлуулалтын захиалга, материалын хүсэлтийг нэгтгэн тодорхой хугацааны Ажлын захиалга, худалдан авалтын шаардлагыг төлөвлөдөг баримт. | Үйлдвэрлэл |
| **Quality Inspection** | **Чанарын үзлэг** | Ирсэн, үйл явц дахь, гарч буй барааг тодорхойлсон хүлээн авах шалгуурт нийцэж байгаа эсэхийг шалгах албан хяналт. | Чанар / Нөөц |
| **Raw Material** | **Түүхий эд** | Дуусгавар буюу хагас боловсруулсан бүтээгдэхүүн үйлдвэрлэхэд хэрэглэдэг боловсруулаагүй эсвэл хамгийн бага боловсруулсан оролтын бараа. | Үйлдвэрлэл / Нөөц |
| **Routing** | **Маршрут** | BOM-ийн үйлдвэрлэлийн зам (ажлын байртай холбосон үйл ажиллагааны дараалал) тодорхойлдог. | Үйлдвэрлэл |
| **Scrap** | **Хаягдал** | Үйлдвэрлэлийн явцад хаях эсвэл үүссэн материал; үйлдвэрлэлийн өртөгт нөлөөлж болох үлдэгдэл үнэ цэнэтэй байж болно. | Үйлдвэрлэл |
| **Serial No** | **Цуврал дугаар** | Барааны нэгж бүрт оноосон давтагдашгүй тодорхойлогч; амьдралын мөчлөгийн туршид (худалдан авалт → борлуулалт → баталгаат хугацаа) бүрэн мөшгих боломжийг олгодог. | Нөөц |
| **Subcontracting** | **Гэрээт үйлдвэрлэл** | Тодорхой үйл ажиллагаа буюу угсралтыг гуравдагч этгээдийн нийлүүлэгчид гаргах тохиолдолд хэрэглэдэг үйлдвэрлэлийн зохицуулалт; нийлүүлэгч түүхий эд хүлээн авч, дуусгавар бүтээгдэхүүн буцааж өгнө. | Үйлдвэрлэл / Худалдан авалт |
| **Work Order** | **Ажлын захиалга** | BOM-ийн дагуу тодорхой тоо хэмжээний барааг үйлдвэрлэхийг зөвшөөрдөг, материалын хэрэглээг хянаж, бодит болон төлөвлөсөн цагийг бүртгэдэг үйлдвэрлэлийн заавар баримт. | Үйлдвэрлэл |
| **Workstation** | **Ажлын байр** | Тодорхой үйлдвэрлэлийн үйл ажиллагаа гүйцэтгэдэг физик эсвэл логик үйлдвэрлэлийн байршил (машин, ширээ, шугам); хүчин чадал болон өртгийн төлөвлөлтөд ашиглагдана. | Үйлдвэрлэл |

---

*Энэхүү тайлбар толь нь `main.pot` орчуулгын загвар файлуудаас автоматаар үүсгэгдсэн бөгөөд тайлбарууд нь Frappe framework болон түүний аппликейшнуудын хэрэглээний нөхцлийг тусгасан болно.*
