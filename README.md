# dapperden.store
Orignal perfumes&amp;accsesories
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>hello to dapper den</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>dapper den</h1>
    <p>orignal perfumes and accsesories</p>
  </header>

  <section class="about">
    <h2>من نحن</h2>
    <p>نحن نقدم أفضل العطور والإكسسوارات الأصلية بتصميم أنيق وجودة عالية.</p>
  </section>

  <footer>
    <p>© 2025 دابر دن. جميع الحقوق محفوظة.</p>
  </footer>
</body>
</html>
body {
  font-family: 'Tahoma', sans-serif;
  margin: 0;
  padding: 0;
  background: #f9f9f9;
  color: #333;
  direction: rtl;
}

header {
  background: #222;
  color: white;
  text-align: center;
  padding: 40px 20px;
}

.about {
  padding: 20px;
  max-width: 800px;
  margin: auto;
}

footer {
  background: #eee;
  text-align: center;
  padding: 20px;
  font-size: 14px;
}
pages:
  stage: deploy
  script:
    - mkdir .public
    - cp -r * .public
    - mv .public public
  artifacts:
    paths:
      - public
  only:
    - main
