# Frappe.MN — Mongolian Translation Glossary

**Apps covered:** ERPNext · Frappe Framework · HRMS · Mail · LMS · Helpdesk  
**Last updated:** 2026-05-09  
**Scope:** Authoritative reference for translators and localisation developers.  
This file governs how terms are translated across all `mn.po` files. When a term
appears here, use the listed translation — do not improvise alternatives.

---

## 1. Conventions

### 1.1 General rules

- **UI labels** (field names, button labels, menu items) use **noun forms** — not verbs.  
  ✓ `Илгээх` (Submit)  ✗ `Оруулах` (which means "to enter/input")
- **Error and warning messages** use complete sentences with a period at the end.
- **Placeholders** `{0}`, `{1}`, `%(name)s` must be preserved exactly as-is.
- **Capitalisation:** Follow the English source — if the English is title-case, use consistent Mongolian capitalisation. Do not ALL-CAPS Mongolian words.
- **Abbreviations:** Keep technical abbreviations (`API`, `PDF`, `HTML`, `BOM`, `UOM`) in English — see §2 below.
- **Do not leave English stems inside Mongolian grammar.** Strings like `Enter a title уу`, `Delete this ticket хийхийг та итгэлтэй байна уу?`, `Refresh session амжилтгүй боллоо` are invalid. Translate the full phrase, not just the suffix.
- **Use one preferred Mongolian form consistently** for repeated technical nouns. In this glossary: `домен` is preferred over `домайн`; `диаграмм` over `диаграм`; `синхрончлох` / `синхрончлол` over bare `синк хийх` in user-facing text.
- **Field labels ending in `ID` keep `ID`** unless the source explicitly means a numeric serial number (`Number`, `No.`). Example: `Email ID`, `GitHub ID`, `OAuth Client ID`.

### 1.2 Document lifecycle states
ERPNext documents pass through states. Use these translations consistently:

| State | Монгол | Notes |
|-------|--------|-------|
| Draft | Ноорог | A document not yet submitted. **Not** `Төсөл` (= project/plan). |
| Submitted | Баталгаажсан | Finalized, cannot be edited without amendment. |
| Cancelled | Цуцлагдсан | Reversed after submission. |
| Amended | Өөрчлөгдсөн | A new version created after cancellation. |
| Approved | Зөвшөөрсөн | A leave/expense that has been approved. |
| Rejected | Татгалзсан | |
| Open | Нээлттэй | |
| Closed | Хаагдсан | |

### 1.3 Action verbs (buttons)
| Action | Монгол | Notes |
|--------|--------|-------|
| Submit | Батлах | Finalizing a document. **Not** `Илгээх` (= to send/email) or `Оруулах` (= to enter). |
| Cancel | Цуцлах | Reversing a submitted document. |
| Amend | Засварлах | Opening a submitted document for editing. |
| Save | Хадгалах | |
| Delete | Устгах | |
| Print | Хэвлэх | |
| Send | Илгээх | Sending an email or message. |
| Assign | Оноох / Даалгах | |
| Export | Экспорт хийх | |
| Import | Импорт хийх | |

### 1.4 Common message templates

Use these sentence patterns for repeated UI strings. Do not translate them word-by-word.

| English pattern | Монгол pattern | Notes |
|-----------------|----------------|-------|
| Are you sure you want to delete this ticket? | Энэ хүсэлтийг устгахдаа итгэлтэй байна уу? | Confirmation dialogs should be fully Mongolian. |
| Enter a valid email address. | Хүчинтэй имэйл хаяг оруулна уу. | Use imperative Mongolian, not `Enter ... уу`. |
| Select a user. | Хэрэглэгч сонгоно уу. | Same rule for `Select`, `Choose`, `Pick`. |
| {0} not found. | {0} олдсонгүй. | Translate `{0}` when it is a normal UI noun. |
| Failed to load {0}. | {0}-г ачаалж чадсангүй. | Prefer a natural Mongolian verb phrase over `Load {0} амжилтгүй боллоо`. |
| Unable to update {0}. | {0}-г шинэчлэх боломжгүй. | Use `боломжгүй` only after a translated verb phrase. |

---

## 2. Do Not Translate

These terms **must stay in English** in all translations. Mongolian users in ERP/tech contexts recognise and expect them in English.

| Term | Reason |
|------|--------|
| `API`, `REST`, `OAuth`, `LDAP`, `JWT`, `SSO` | Technical protocols — no accepted Mongolian equivalent |
| `HTML`, `CSS`, `JavaScript`, `Python`, `JSON`, `CSV`, `PDF`, `XML` | File formats and languages |
| `ID`, `URL`, `OAuth Client ID`, `Client Secret` | Technical identifiers and credentials |
| `DocType` | Frappe-specific concept — translating would break documentation links |
| `BOM`, `SKU`, `UOM`, `FIFO`, `POS` | Industry abbreviations used universally in ERP |
| `DKIM`, `DMARC`, `SPF`, `SMTP`, `IMAP` | Email authentication standards |
| `SLA` | Use full form `Үйлчилгээний түвшний гэрээ` on first mention in help text; in labels keep `SLA` |
| `ERPNext`, `Frappe`, `HRMS`, `LMS`, `CRM`, `ERP` | Brand/product names |
| `Google`, `Microsoft`, `GitHub`, `Stripe`, `PayPal`, `Zoom`, `WhatsApp`, `Gmail`, `Outlook` | Brand names |
| `Jinja`, `Bootstrap`, `Vue`, `React`, `Redis`, `Ansible` | Software libraries |
| `Email` | Universally understood; `Имэйл` is acceptable in prose but `Email` in field labels |

---

## 3. Disambiguation — Critical Pairs

These are the most common source of translation errors. The wrong choice changes the meaning of the UI.

### Customer vs. User
| English | Монгол | When to use |
|---------|--------|-------------|
| **Customer** | **Харилцагч** | A business entity that buys goods/services (Sales, CRM). |
| **User** | **Хэрэглэгч** | A person with a login account in the system. |
| **Client** | **Үйлчлүүлэгч** | In professional services or legal context. |

> ⚠️ Do **not** use `Хэрэглэгч` for `Customer`. In ERP, these are distinct records.

### Stock vs. Shares
| English | Монгол | When to use |
|---------|--------|-------------|
| **Stock** (inventory) | **Нөөц** | Physical goods in a warehouse. |
| **Stock** (financial shares) | **Хувьцаа** | Equity shares in a company — rare in ERPNext context. |

### Leave vs. Departure

| English | Монгол | When to use |
|---------|--------|-------------|
| **Leave** (HR) | **Чөлөө** | Approved absence from work (sick leave, annual leave). |
| **Leave** (to depart) | **Явах** | Action of leaving — not used in HR module labels. |

### Rate vs. Rating
| English | Монгол | When to use |
|---------|--------|-------------|
| **Rate** (price per unit) | **Тариф** | Unit price on invoice/BOM lines. |
| **Rating** (score) | **Үнэлгээ** | Star rating, performance score. |
| **Exchange Rate** | **Ханш** | Currency conversion rate specifically. |

### Issue vs. Stock Issue
| English | Монгол | When to use |
|---------|--------|-------------|
| **Issue** (support ticket) | **Асуудал** | Helpdesk/project issue. |
| **Issue** (stock transfer out) | **Гаргалт** | Inventory movement out of warehouse. |

### Submit vs. Send
| English | Монгол | When to use |
|---------|--------|-------------|
| **Submit** (document) | **Батлах** | Finalizing/locking an ERPNext document. |
| **Send** (email/message) | **Илгээх** | Dispatching a communication. |

> ⚠️ These were previously mixed up in `hrms/mn.po`. `Permanently submit {0}` = `{0}-г байнга батлах`, not `оруулах`.

### Draft vs. Project
| English | Монгол | When to use |
|---------|--------|-------------|
| **Draft** (document state) | **Ноорог** | A document that has not been submitted. |
| **Project** | **Төсөл** | A project with tasks and milestones. |

> ⚠️ `DRAFT` watermark on print formats must be `НООРОГ`, not `ТӨСӨЛ`.

### Advance vs. Progress
| English | Монгол | When to use |
|---------|--------|-------------|
| **Advance** (prepayment) | **Урьдчилгаа** | Advance payment made before work/delivery. |
| **Progress** | **Явц** | Progress of a task or project. |

---

## 4. Term Reference

### Accounting & Finance

| English | Монгол | Notes |
|---------|--------|-------|
| Account | Данс | |
| Accountant | Нягтлан бодогч | |
| Accounting | Нягтлан бодох бүртгэл | |
| Accounts Payable | Дансны өглөг | Money owed to suppliers |
| Accounts Receivable | Дансны авлага | Money owed by customers |
| Accrued Expenses | Хуримтлагдсан зардал | |
| Accumulated Depreciation | Хуримтлагдсан элэгдэл | |
| Advance Payment | Урьдчилгаа төлбөр | See §3: Advance vs. Progress |
| Asset | Хөрөнгө | |
| As On Date / As on Date | Тухайн огноогоор | Report filter — "as of this date" |
| Balance Sheet | Баланс | |
| Bank Account | Банкны данс | |
| Bank Reconciliation | Банкны нэгтгэл | |
| Bank Transaction | Банкны гүйлгээ | |
| Budget | Төсөв | |
| Budget Variance | Төсвийн зөрүү | |
| Cash Flow | Мөнгөн урсгал | |
| Chart of Accounts | Дансны мод | Align with Odoo Mongolian; **not** `Дансны график` |
| Closing Balance | Эцсийн үлдэгдэл | |
| Cost Center | Зардлын төв | |
| Cost of Goods Sold | Борлуулсан бүтээгдэхүүний өртөг | |
| Credit | Кредит | Keep as-is (accounting term) |
| Credit Note | Зээлийн тэмдэглэл | |
| Currency | Валют | |
| Debit | Дебит | Keep as-is (accounting term) |
| Debit Note | Дебит тэмдэглэл | |
| Depreciation | Элэгдэл | |
| Equity | Өмч | |
| Exchange Rate | Ханш | See §3: Rate vs. Rating |
| Expense | Зардал | |
| Fiscal Year | Санхүүгийн жил | |
| Fixed Asset | Үндсэн хөрөнгө | |
| General Ledger | Ерөнхий дэвтэр | |
| Gross Profit | Нийт ашиг | |
| Invoice | Нэхэмжлэх | |
| Journal Entry | Ажил гүйлгээ | Align with Odoo Mongolian; `Journal Item` = `Журналын бичилт` |
| Liabilities | Өр төлбөр | |
| Net Profit | Цэвэр ашиг | |
| Opening Balance | Эхний үлдэгдэл | |
| Outstanding Amount | Хаагдаагүй дүн | Amount not yet paid |
| Payment | Төлбөр | |
| Payment Entry | Төлбөрийн бичилт | |
| Payment Terms | Төлбөрийн нөхцөл | |
| Profit and Loss | Ашиг алдагдлын тайлан | Use `&` only in tab labels: `Ашиг & алдагдал` |
| Purchase Invoice | Худалдан авалтын нэхэмжлэх | |
| Rate & Amount | Тариф & Дүн | BOM line — unit price and total |
| Revenue | Орлого | |
| Sales Invoice | Борлуулалтын нэхэмжлэх | |
| Tax | Татвар | |
| Tax Withholding | Суутган татвар | |
| Trial Balance | Туршилтын баланс | |
| Write Off | Хасах | |

### Sales & CRM

| English | Монгол | Notes |
|---------|--------|-------|
| Campaign | Кампанит ажил | |
| Commission | Шимтгэл | |
| Contact | Холбогч хүн | |
| Customer | Харилцагч | See §3 — **not** `Хэрэглэгч` |
| Customer Group | Харилцагчийн бүлэг | |
| Delivery Note | Хүргэлтийн баримт | |
| Discount | Хөнгөлөлт | |
| Lead | Боломжит харилцагч | "Lead" in CRM; not `Тэргүүлэх` (= leading/priority) |
| Opportunity | Боломж | |
| Price List | Үнийн жагсаалт | |
| Quotation | Үнийн санал | |
| Sales Order | Борлуулалтын захиалга | |
| Sales Person | Борлуулалтын ажилтан | |
| Sales Return | Буцаалт | |
| Shipment | Тээвэрлэлт | |
| Territory | Нутаг дэвсгэр | |

### Purchasing

| English | Монгол | Notes |
|---------|--------|-------|
| Material Request | Материалын хүсэлт | |
| Purchase Invoice | Худалдан авалтын нэхэмжлэх | |
| Purchase Order | Худалдан авалтын захиалга | |
| Purchase Receipt | Худалдан авалтын хүлээн авалт | |
| Request for Quotation | Үнийн санал авах хүсэлт | |
| Subcontracting | Гэрээт үйлдвэрлэл | |
| Supplier | Нийлүүлэгч | |
| Supplier Quotation | Нийлүүлэгчийн үнийн санал | |

### Inventory & Warehouse

| English | Монгол | Notes |
|---------|--------|-------|
| Batch | Бүлэг | Lot/batch of items |
| Bill of Materials | Материалын жагсаалт | Abbreviated as `BOM` — keep abbreviation |
| Delivery Note | Хүргэлтийн баримт | |
| Expiry Date | Дуусгавар болох огноо | |
| FIFO | FIFO | Keep abbreviation; spell out in help text: "Эхэлж орсон эхэлж гарна" |
| Inventory | Нөөц | |
| Item | Зүйл | Generic; in product contexts `Бараа` is also acceptable |
| Item Code | Барааны код | |
| Item Group | Барааны бүлэг | |
| Material Transfer | Материалын шилжүүлэг | |
| Putaway Rule | Байршуулах дүрэм | |
| Reorder Level | Дахин захиалах түвшин | |
| Reserved Stock | Нөөцлөгдсөн бараа | |
| Stock | Нөөц | Inventory stock — see §3 for shares |
| Stock Entry | Нөөцийн бичилт | |
| Stock Ledger | Нөөцийн дэвтэр | |
| UOM / Unit of Measure | Хэмжлийн нэгж | Keep `UOM` as abbreviation in labels |
| Valuation | Үнэлгээ | Inventory valuation method |
| Warehouse | Агуулах | |

### Common UI & Profile Fields

| English | Монгол | Notes |
|---------|--------|-------|
| Chart | Диаграмм | Visual chart/widget; do not use `диаграм`. |
| Dashboard Chart | Хяналтын самбарын диаграмм | |
| Email ID | Email ID | Keep `ID`; do not translate as `Email дугаар`. |
| First Name | Нэр | |
| Full Name | Бүтэн нэр | Prefer this over mixed forms like `Full нэр`. |
| Gantt | Гант | In labels like `Gantt View`; avoid `диаграммм`. |
| Gantt View | Гант харагдац | |
| GitHub ID | GitHub ID | Keep brand + `ID`. |
| Last Name | Овог | Do not leave `Last нэр`. |
| Session | Сесс | Technical login/session context. |
| Sync | Синхрончлох / Синхрончлол | Verb / noun form. Avoid raw `синк хийх` in user-facing copy. |
| View | Харагдац | Noun sense: saved view, list view, calendar view. Verb `View` = `Харах`. |

### HR & Payroll

| English | Монгол | Notes |
|---------|--------|-------|
| Appraisal | Ажлын үнэлгээ | Performance review |
| Attendance | Ирц | |
| Bonus | Урамшуулал | |
| Deduction | Суутгал | Salary deduction |
| Department | Хэлтэс | |
| Designation | Албан тушаал | Job title |
| Employee | Ажилтан | |
| Employee Onboarding | Ажилтныг элсүүлэх | |
| Expense Claim | Зардлын нэхэмжлэл | |
| Gratuity | Ажиллах хугацааны тэтгэмж | End-of-service benefit |
| Holiday | Амралт | Public holiday or day off |
| Holiday List | Амралтын жагсаалт | |
| Income Tax Slab | Орлогын татварын шат | |
| Job Applicant | Ажил горилогч | |
| Job Opening | Ажлын байрны зар | |
| Leave | Чөлөө | See §3 — HR absence, not departure |
| Leave Allocation | Чөлөөний хуваарилалт | |
| Leave Application | Чөлөөний өргөдөл | |
| Leave Without Pay | Цалингүй чөлөө | |
| Notice Period | Мэдэгдлийн хугацаа | |
| Overtime | Илүү цагийн ажил | |
| Payroll | Цалин хөлс | The payroll process |
| Salary | Цалин | The amount paid |
| Salary Component | Цалингийн бүрэлдэхүүн | |
| Salary Slip | Цалингийн хуудас | Payslip |
| Salary Structure | Цалингийн бүтэц | |
| Shift | Ээлж | Work shift |
| Training | Сургалт | |

### Manufacturing

| English | Монгол | Notes |
|---------|--------|-------|
| BOM | Материалын жагсаалт (BOM) | Keep `BOM` abbreviation alongside |
| Capacity Planning | Хүчин чадлын төлөвлөлт | |
| Downtime | Сул зогсолт | |
| Job Card | Ажлын карт | |
| Production Plan | Үйлдвэрлэлийн төлөвлөгөө | |
| Quality Inspection | Чанарын үзлэг | |
| Routing | Маршрут | |
| Scrap | Хаягдал | |
| Work Order | Ажлын захиалга | |
| Workstation | Ажлын байр | |

### System & Access Control

| English | Монгол | Notes |
|---------|--------|-------|
| Administrator | Администратор | |
| Dashboard | Хяналтын самбар | |
| DocType | DocType | Do not translate — see §2 |
| Document | Баримт | An ERPNext record |
| Error Log | Алдааны бүртгэл | |
| Module | Модуль | |
| Notification | Мэдэгдэл | |
| Permission | Зөвшөөрөл | |
| Report | Тайлан | **Not** `мэдээлэх` (= "to inform", a verb) |
| Role | Үүрэг | System role; **not** `Дүр` (= theatrical role) |
| Translate / Translation | Орчуулга | |
| Two Factor Authentication | Хоёр шатлалт баталгаажуулалт | |
| User | Хэрэглэгч | System login account — see §3 |
| Webhook | Webhook | Do not translate |
| Workflow | Ажлын урсгал | |
| Workspace | Ажлын талбар | |

### Mail (Frappe Mail)

| English | Монгол | Notes |
|---------|--------|-------|
| Alias | Өөр нэр | Alternative address |
| Attachment | Хавсралт | |
| Contact HTML | Холбоо барих HTML | Field/section label; not an instruction sentence. |
| Domain | Домен | Preferred spelling; plural `доменууд`. |
| Draft | Ноорог | See §3 — **not** `Төсөл` |
| Inbox | Ирсэн хайрцаг | |
| Mail Queue | Шуудангийн дараалал | |
| Mailbox | Шуудангийн хайрцаг | |
| Newsletter | Мэдээллийн товхимол | |
| Root Domain Name | Үндсэн домен нэр | |
| Signup Domains | Бүртгэлийн доменууд | Domains allowed for signup/registration |
| Signature | Гарын үсэг | Email signature |
| Spam | Хог шуудан | |
| Thread | Хэлхээ | Email conversation thread |

### Helpdesk

| English | Монгол | Notes |
|---------|--------|-------|
| Agent | Оператор | Support agent; **not** `Агент` (= secret agent) |
| Knowledge Base | Мэдлэгийн сан | |
| Rating | Үнэлгээ | Customer satisfaction score — see §3 |
| Resolution | Шийдвэрлэлт | |
| SLA | SLA | Keep abbreviation; spell out in help text |
| Ticket | Хүсэлт | Support request; `(тикет)` may be added in parentheses for clarity |
| Ticket Priority | Хүсэлтийн тэргүүлэх зэрэглэл | |

### Learning (LMS)

| English | Монгол | Notes |
|---------|--------|-------|
| Assessment | Үнэлгээ | |
| Batch | Бүлэг | Student cohort |
| Certificate | Гэрчилгээ | |
| Chapter | Бүлэг | Course chapter; context distinguishes from student batch |
| Course | Курс | **Not** `мэдээж` (= "obviously/of course" — wrong word entirely) |
| Instructor | Багш / Зааварлагч | |
| Lesson | Хичээл | |
| Quiz | Шалгалт | |
| Student | Оюутан | |
