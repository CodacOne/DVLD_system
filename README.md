# 🚗 DVLD - نظام إدارة رخص القيادة

نظام تدريبي لإدارة عمليات ترخيص السائقين والمركبات، يشمل إصدار وتجديد واستبدال الرخص، وإدارة الاختبارات وفئات الرخص والمستخدمين، مع تنظيم البيانات بشكل احترافي ومتوافق مع المتطلبات الواقعية لإدارات المرور.

---

## 🧰 التقنيات المستخدمة

- 💻 C# - Windows Forms
- 🗃️ SQL Server
- 🏗️ 3-Tier Architecture

---

## 🧾 وصف النظام

يقدم النظام خدمات متنوعة تخص إدارة رخص القيادة، ويتم التعامل مع الطلبات وفقًا لمجموعة من الشروط المسبقة والمتطلبات القانونية. يعتمد النظام على قاعدة بيانات مركزية ويتميز بفصل الطبقات (Presentation - Business Logic - Data Access) لسهولة الصيانة والتطوير.

---

## 🧩 المزايا الرئيسية

### 📄 الطلبات المدعومة:

| الخدمة | رسوم الطلب |
|--------|------------|
| إصدار رخصة لأول مرة | 5$ |
| إعادة فحص | 5$ |
| تجديد الرخصة | 5$ |
| إصدار بدل فاقد | 5$ |
| إصدار بدل تالف | 5$ |
| فك حجز رخصة | 5$ |
| إصدار رخصة دولية | 5$ |

> 📝 ملاحظات:
> - رسوم الفحوصات والرخص تُضاف إلى رسوم الطلب.
> - يُمنع تكرار نفس نوع الطلب إن لم يُستكمل سابقًا.

---

### 🧑‍💼 معلومات مقدم الطلب:

- الرقم الوطني (أساسي وفريد)
- الاسم الرباعي
- تاريخ الميلاد
- العنوان
- الهاتف
- البريد الإلكتروني
- الجنسية
- الصورة الشخصية

---

### 🪪 فئات رخص القيادة

| الفئة | الوصف | الحد الأدنى للعمر | رسوم الرخصة | مدة الصلاحية |
|-------|-------|-------------------|--------------|----------------|
| الأولى | دراجات نارية صغيرة | 18 | 15$ | 5 سنوات |
| الثانية | دراجات نارية ثقيلة | 21 | 30$ | 5 سنوات |
| الثالثة | مركبات خفيفة / سيارات | 18 | 20$ | 10 سنوات |
| الرابعة | سيارات أجرة / ليموزين | 21 | 200$ | 10 سنوات |
| الخامسة | مركبات زراعية | 21 | 50$ | 10 سنوات |
| السادسة | حافلات صغيرة ومتوسطة | 21 | 250$ | 10 سنوات |
| السابعة | شاحنات ومركبات ثقيلة | 21 | 300$ | 10 سنوات |

---

### 🧪 اختبارات الرخصة:

1. **اختبار النظر** – رسوم: 10$
2. **الاختبار النظري** – رسوم: 20$ (علامة من 100)
3. **الاختبار العملي** – حسب الفئة

- لا يمكن التقديم لاختبار لاحق دون النجاح في الاختبار السابق.
- تُسجل جميع النتائج والمواعيد في النظام.

---

## 📋 خدمات إضافية

- **إصدار رخصة دولية**:
  - فقط لحاملي رخص الفئة الثالثة.
  - يجب أن تكون الرخصة سارية وغير محجوزة.
  - لا يمكن إصدار أكثر من رخصة دولية فعالة.

- **إعادة فحص**:
  - متاحة فقط بعد الرسوب.
  - ترتبط بالطلب الأصلي.

- **فك الحجز**:
  - يتطلب دفع الغرامة وتسجيل تاريخ فك الحجز.

---

## 🔐 إدارة النظام

### 👤 إدارة المستخدمين:
- إضافة/تعديل/تجميد/حذف
- ربط كل مستخدم بشخص حقيقي في النظام
- إعطاء صلاحيات

### 👥 إدارة الأشخاص:
- منع تكرار الرقم الوطني
- تعديل البيانات
- البحث بالرقم الوطني

### 📄 إدارة الطلبات:
- فلترة حسب الحالة
- ربط الطلب بشخص
- تعديل رسوم الطلبات

### 🛠️ إدارة الفئات والاختبارات:
- الفئات ثابتة ويمكن تعديل خصائصها.
- يمكن تعديل رسوم الاختبارات فقط.

---

## ▶️ كيفية التشغيل

1. افتح المشروع باستخدام Visual Studio.
2. عدّل إعدادات الاتصال بقاعدة البيانات.
3. حدّث بيانات المستخدمين.
4. شغّل التطبيق وتفاعل مع الواجهات الرسومية (Windows Forms).

### بيانات تسجيل الدخول (للنسختين العربية والإنجليزية):

| اسم المستخدم | كلمة المرور |
|--------------|-------------|
| a            | a           |
---

## 📸 لقطات شاشة (اختياري)

> *يمكنك هنا إضافة صور من واجهات النظام (Forms) لتوضيح العمل.*

---

## 🧑‍💻 المؤلف

**Abdulftah Kashkash**  
💼 مهندس تحكم وأتمتة صناعية  
💻 مطور C# .NET  
📧 abdulftah.dev@example.com (تعديل)

---

© 2025 Abdulftah Kashkash – جميع الحقوق محفوظة.


# 🚗 DVLD - Driving & Vehicle License Department System

A training system for managing driver and vehicle licensing operations, including issuance, renewal, replacement of licenses, test management, license classes, and user management. The system follows realistic requirements for traffic licensing departments.

---

## 🧰 Technologies Used

- 💻 C# - Windows Forms
- 🗃️ SQL Server
- 🏗️ 3-Tier Architecture

---

## 🧾 System Description

The system offers various services related to driver license management. Requests are handled according to predefined legal conditions and requirements. The system uses a centralized database and employs separation of layers (Presentation - Business Logic - Data Access) for easy maintenance and development.

---

## 🧩 Main Features

### 📄 Supported Requests:

| Service | Request Fee |
|---------|-------------|
| New License Issuance | $5 |
| Retest | $5 |
| License Renewal | $5 |
| Lost License Replacement | $5 |
| Damaged License Replacement | $5 |
| License Unblocking | $5 |
| International License Issuance | $5 |

> 📝 Notes:
> - Additional fees for tests and licenses apply.
> - Duplicate incomplete requests of the same type are prevented.

---

### 🧑‍💼 Applicant Information:

- National ID (unique key)
- Full Name
- Date of Birth
- Address
- Phone Number
- Email
- Nationality
- Personal Photo

---

### 🪪 License Classes

| Class | Description | Minimum Age | License Fee | Validity Period |
|-------|-------------|-------------|-------------|-----------------|
| 1st | Small Motorcycles | 18 | $15 | 5 years |
| 2nd | Heavy Motorcycles | 21 | $30 | 5 years |
| 3rd | Light Vehicles / Cars | 18 | $20 | 10 years |
| 4th | Commercial Vehicles (Taxi/Limousine) | 21 | $200 | 10 years |
| 5th | Agricultural Vehicles | 21 | $50 | 10 years |
| 6th | Small and Medium Buses | 21 | $250 | 10 years |
| 7th | Trucks and Heavy Vehicles | 21 | $300 | 10 years |

---

### 🧪 License Tests:

1. **Vision Test** – Fee: $10  
2. **Theoretical Test** – Fee: $20 (Score out of 100)  
3. **Practical Driving Test** – Fee varies by license class

- Applicants must pass each test before proceeding to the next.
- All results and appointments are recorded in the system.

---

## 📋 Additional Services

- **International License Issuance**:  
  - Available only to holders of the 3rd class license.  
  - License must be valid and not blocked.  
  - Only one active international license allowed; issuing a new one cancels the previous and keeps a record.

- **Retesting**:  
  - Allowed only after failure.  
  - Linked to the original request.

- **License Unblocking**:  
  - Requires payment of fines and recording unblock date.

---

## 🔐 System Administration

### 👤 User Management:
- Add/Edit/Freeze/Delete users
- Link users to real persons in the system
- Assign permissions

### 👥 Person Management:
- Prevent duplicate National IDs
- Edit personal data
- Search by National ID

### 📄 Request Management:
- Filter by request status
- Link request to person
- Edit request fees

### 🛠️ License Classes & Tests Management:
- License classes are fixed but properties can be edited.
- Test fees are adjustable.

---

## ▶️ How to Run

- Open the project in Visual Studio.
- Update the database connection string.
- Seed the system with users.
- Run the application and log in.

### Login Credentials (for both Arabic & English versions):

| Username | Password |
|----------|----------|
| a        | a        |

---

## 📸 Screenshots (Optional)

*Add screenshots of system forms here to showcase the UI.*

---

## 🧑‍💻 Author

**Abdulftah Kashkash**  
💼 Control & Automation Engineer  
💻 C# .NET Developer  
📧 abdulftah.dev@example.com (placeholder)

---

© 2025 Abdulftah Kashkash – All rights reserved.
