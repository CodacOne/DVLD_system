<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>DVLD - نظام إدارة وإصدار رخص السائقين</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
      background-color: #f9f9f9;
      color: #222;
    }
    h1, h2, h3 {
      color: #2c3e50;
      margin-bottom: 10px;
    }
    h1 {
      font-size: 2.2em;
    }
    ul {
      margin: 0 0 15px 20px;
    }
    li {
      margin-bottom: 8px;
    }
    p {
      margin: 12px 0;
    }
    .en-text {
      direction: ltr;
      font-style: italic;
      color: #555;
      margin: 8px 0 20px 0;
    }
    footer {
      margin-top: 40px;
      border-top: 1px solid #ddd;
      padding-top: 10px;
      font-size: 0.9em;
      color: #888;
      text-align: center;
    }
  </style>
</head>
<body>

  <h1>🚗 نظام إدارة وإصدار رخص السائقين (DVLD)</h1>
  <p><strong>نظام تدريبي لإدارة رخص السائقين</strong> تم تطويره باستخدام <code>C#</code> و<code>Windows Forms</code> مع قاعدة بيانات <code>SQL Server</code> ضمن بنية <strong>3-Tier Architecture</strong>.</p>
  <p class="en-text"><strong>Training system for Driving License Management</strong> developed with <code>C#</code>, <code>Windows Forms</code>, and <code>SQL Server</code> following a <strong>3-Tier Architecture</strong>.</p>

  <h2>📋 نظرة عامة</h2>
  <p>يهدف النظام إلى إدارة جميع عمليات إصدار وتجديد واستبدال رخص القيادة مع الالتزام بالشروط الخاصة بكل فئة رخصة.</p>
  <p class="en-text">The system manages all processes related to issuing, renewing, and replacing driving licenses while enforcing category-specific requirements.</p>

  <h2>🧾 الخدمات الرئيسية:</h2>
  <ul>
    <li>إصدار رخصة قيادة لأول مرة</li>
    <p class="en-text">Issuance of a new driving license</p>

    <li>إعادة الفحص</li>
    <p class="en-text">Re-examination</p>

    <li>تجديد رخصة القيادة</li>
    <p class="en-text">License renewal</p>

    <li>إصدار بدل رخصة مفقودة أو تالفة</li>
    <p class="en-text">Issuance of replacement for lost or damaged licenses</p>

    <li>فك حجز الرخصة</li>
    <p class="en-text">Release of license detention</p>

    <li>إصدار رخصة دولية</li>
    <p class="en-text">Issuance of international driving license</p>
  </ul>

  <h2>💲 الرسوم</h2>
  <ul>
    <li>رسوم تقديم الخدمة: 5 دولارات لكل خدمة</li>
    <p class="en-text">Service fee: $5 per service</p>

    <li>رسوم الفحوصات: تختلف حسب نوع الفحص والفئة</li>
    <p class="en-text">Examination fees vary by type and license category</p>

    <li>رسوم الرخص: تعتمد على فئة الرخصة المطلوبة</li>
    <p class="en-text">License fees depend on the requested license category</p>
  </ul>

  <h2>🪪 فئات رخص القيادة</h2>
  <ul>
    <li>الفئة الأولى: دراجات نارية صغيرة - 15 دولار - العمر 18 - صلاحية 5 سنوات</li>
    <p class="en-text">Category 1: Small motorcycles - $15 - Age 18+ - Valid for 5 years</p>

    <li>الفئة الثانية: دراجات نارية كبيرة - 30 دولار - العمر 21 - صلاحية 5 سنوات</li>
    <p class="en-text">Category 2: Large motorcycles - $30 - Age 21+ - Valid for 5 years</p>

    <li>الفئة الثالثة: المركبات الخفيفة - 20 دولار - العمر 18 - صلاحية 10 سنوات</li>
    <p class="en-text">Category 3: Light vehicles - $20 - Age 18+ - Valid for 10 years</p>

    <li>الفئة الرابعة: سيارات أجرة/ليموزين - 200 دولار - العمر 21 - صلاحية 10 سنوات</li>
    <p class="en-text">Category 4: Taxi/Limousine - $200 - Age 21+ - Valid for 10 years</p>

    <li>الفئة الخامسة: مركبات زراعية - 50 دولار - العمر 21 - صلاحية 10 سنوات</li>
    <p class="en-text">Category 5: Agricultural vehicles - $50 - Age 21+ - Valid for 10 years</p>

    <li>الفئة السادسة: حافلات صغيرة ومتوسطة - 250 دولار - العمر 21 - صلاحية 10 سنوات</li>
    <p class="en-text">Category 6: Small and medium buses - $250 - Age 21+ - Valid for 10 years</p>

    <li>الفئة السابعة: شاحنات ومركبات ثقيلة - 300 دولار - العمر 21 - صلاحية 10 سنوات</li>
    <p class="en-text">Category 7: Trucks and heavy vehicles - $300 - Age 21+ - Valid for 10 years</p>
  </ul>

  <h2>📌 متطلبات الحصول على الرخصة</h2>
  <ul>
    <li>تقديم المستندات الشخصية اللازمة</li>
    <p class="en-text">Submission of required personal documents</p>

    <li>التحقق من السن المناسب لكل فئة</li>
    <p class="en-text">Age verification according to category</p>

    <li>عدم وجود رخصة نشطة من نفس الفئة</li>
    <p class="en-text">No active license of the same category</p>

    <li>اجتياز الفحوصات الطبية والنظرية والعملية</li>
    <p class="en-text">Passing medical, theoretical, and practical exams</p>
  </ul>

  <h2>📁 إدارة النظام</h2>
  <ul>
    <li>إدارة المستخدمين (إضافة، تعديل، حذف، تجميد، إعطاء صلاحيات)</li>
    <p class="en-text">User management (Add, Edit, Delete, Freeze, Assign permissions)</p>

    <li>إدارة الأشخاص المرتبطين بالنظام</li>
    <p class="en-text">Management of registered persons</p>

    <li>إدارة الطلبات والاختبارات وفئات الرخص</li>
    <p class="en-text">Management of applications, tests, and license categories</p>

    <li>حجز وفك حجز الرخص مع تسجيل بيانات الحجز والغرامات</li>
    <p class="en-text">License detention and release with logging of details and fines</p>
  </ul>

  <h2>💻 التقنيات المستخدمة</h2>
  <ul>
    <li><strong>اللغة الأساسية:</strong> C#</li>
    <p class="en-text"><strong>Main language:</strong> C#</p>

    <li><strong>واجهة المستخدم:</strong> Windows Forms</li>
    <p class="en-text"><strong>UI:</strong> Windows Forms</p>

    <li><strong>قاعدة البيانات:</strong> SQL Server</li>
    <p class="en-text"><strong>Database:</strong> SQL Server</p>

    <li><strong>البنية المعمارية:</strong> 3-Tier Architecture</li>
    <p class="en-text"><strong>Architecture:</strong> 3-Tier Architecture</p>
  </ul>

  <h2>👤 بيانات الدخول التجريبية</h2>
  <ul>
    <li>اسم المستخدم: <code>a</code></li>
    <p class="en-text">Username: <code>a</code></p>

    <li>كلمة المرور: <code>a</code></li>
    <p class="en-text">Password: <code>a</code></p>
  </ul>

  <h2>📌 ملاحظات هامة</h2>
  <p>تم تنفيذ هذا المشروع بشكل فردي كتمرين عملي لبناء نظام إداري متكامل.</p>
  <p class="en-text">This project was developed individually as a practical exercise for building a comprehensive management system.</p>

  <footer>
    <hr />
    <p>© 2023 - ProgrammingAdvices.com</p>
  </footer>

</body>
</html>
