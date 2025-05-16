Phao tk web 
Cau 1: 
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>English Learning</title>
  <style>
    :root {
      --yellow: #ffe700;
      --green-light: #00e56b;
      --green-dark: #00b253;
      --blue-light: #2fcbff;
      --blue-dark: #2f63ff;
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    header {
      background: var(--blue-dark);
      color: white;
      padding: 1rem 2rem;
      display: flex;
      align-items: center;
      gap: 1rem;
      flex-wrap: wrap;
    }

    header svg {
      width: 48px;
      height: 48px;
      flex-shrink: 0;
    }

    .navigation {
      background: var(--blue-light);
      width: 100%;
    }

    .navigation ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      padding: 1rem 2rem;
      justify-content: center;
    }

    .navigation a {
      color: #000;
      text-decoration: none;
      font-weight: bold;
    }

    .navigation a:hover {
      color: white;
    }

    main {
      padding: 2rem;
      max-width: 900px;
      margin: auto;
    }

    main img {
      max-width: 100%;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <header>
    <!-- Logo SVG -->
    <svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" aria-label="English Learning Logo">
      <circle cx="32" cy="32" r="32" fill="#2fcbff"/>
      <text x="32" y="38" font-size="28" text-anchor="middle" fill="#2f63ff" font-family="Arial" font-weight="bold">EL</text>
    </svg>
    <h1>English Learning</h1>
  </header>

  <!-- Navigation bằng div -->
  <div class="navigation">
    <ul>
      <li><a href="#home">Trang chủ</a></li>
      <li><a href="#courses">Khóa học</a></li>
      <li><a href="#about">Giới thiệu</a></li>
      <li><a href="#contact">Liên hệ</a></li>
    </ul>
  </div>

  <!-- Bài viết khóa học -->
  <main>
    <article>
      <h2>Khóa học Tiếng Anh Giao Tiếp Cơ Bản</h2>
      <img src="https://dummyimage.com/800x300/2f63ff/ffffff&text=English+Course" alt="English course banner">
      <p><strong>English Learning</strong> tự hào giới thiệu khóa học <strong>Giao Tiếp Cơ Bản</strong> dành cho người mới bắt đầu. Khóa học tập trung xây dựng nền tảng từ vựng và phát âm chuẩn thông qua phương pháp học tương tác và các hoạt động giao tiếp thực tế.</p>
    </article>
  </main>

</body>
</html>
Cau 2: 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>English Learning</title>
</head>
<style>
    :root {
  --yellow: #ffe700;
  --green-light: #00e56b;
  --green-dark: #00b253;
  --blue-light: #2fcbff;
  --blue-dark: #2f63ff;
  --item-size: 220px;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}
.advert {
  width: 100%;
  height: 200px;
  border: 2px solid var(--blue-dark);
  background: var(--yellow);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.2rem;
  transition: all .3s ease;
}
.item {
  width: var(--item-size);
  height: var(--item-size);
  background: var(--blue-light);
  margin: 0.5rem;
  padding: 1rem;
  border-radius: 12px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
body {
  padding: 2rem;
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
</style>
<body>
        <div class="item">item1</div>
        <div class="item">item2</div>
        <div class="item">item3</div>
        <div class="item">item4</div>
        <div class="advert">Dang ki ngay de nhan khuyen mai</div>
</body>
</html>

Cau 3: 
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<title>Câu 3 - JSON & While Loop</title>
<style>

:root {
  --yellow: #ffe700;
  --green-light: #00e56b;
  --green-dark: #00b253;
  --blue-light: #2fcbff;
  --blue-dark: #2f63ff;
  --item-size: 220px;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}
.item {
  width: var(--item-size);
  height: var(--item-size);
  background: var(--blue-light);
  margin: 0.5rem;
  padding: 1rem;
  border-radius: 12px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.item h3 {
  margin-bottom: .5rem;
}
.items-container {
  max-width: 1200px;
  margin: auto;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
</head>
<body>
<div class="items-container" id="courses"></div>

<script>
const courses = [
  {
    "name": "Basic English",
    "description": "Xây dựng nền tảng từ vựng và ngữ pháp cơ bản.",
    "fee": "3,000,000 VND",
    "start": "2025-06-01"
  },
  {
    "name": "Intermediate Conversation",
    "description": "Nâng cao kỹ năng giao tiếp, phản xạ nhanh.",
    "fee": "4,500,000 VND",
    "start": "2025-06-15"
  },
  {
    "name": "IELTS Intensive",
    "description": "Chuẩn bị IELTS trong 3 tháng với giáo viên bản ngữ.",
    "fee": "8,000,000 VND",
    "start": "2025-07-01"
  },
  {
    "name": "Business English",
    "description": "Kỹ năng tiếng Anh thương mại chuyên sâu.",
    "fee": "6,500,000 VND",
    "start": "2025-07-10"
  }
];

let i = 0;
const container = document.getElementById('courses');
while (i < courses.length) {
  const c = courses[i];
  const div = document.createElement('div');
  div.className = 'item';
  div.innerHTML = `<h3>${c.name}</h3><p>${c.description}</p><p><strong>Học phí:</strong> ${c.fee}</p><p><strong>Khai giảng:</strong> ${c.start}</p>`;
  container.appendChild(div);
  i++;
}
// su dung for-each: const container = document.getElementById('courses');

// courses.forEach(function(c) {
//   const div = document.createElement('div');
//   div.className = 'item';
//   div.innerHTML = `<h3>${c.name}</h3>
//                    <p>${c.description}</p>
//                    <p><strong>Học phí:</strong> ${c.fee}</p>
//                    <p><strong>Khai giảng:</strong> ${c.start}</p>`;
//   container.appendChild(div);
// }); 
// su dung for : const container = document.getElementById('courses');

// for (let i = 0; i < courses.length; i++) {
//   const c = courses[i];
//   const div = document.createElement('div');
//   div.className = 'item';
//   div.innerHTML = `<h3>${c.name}</h3>
//                    <p>${c.description}</p>
//                    <p><strong>Học phí:</strong> ${c.fee}</p>
//                    <p><strong>Khai giảng:</strong> ${c.start}</p>`;
//   container.appendChild(div);
// }
</script>
</body>
</html>
Cau 4: 
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Câu 4 - Form Đăng Ký</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    :root {
      --yellow: #ffe700;
      --green-light: #00e56b;
      --green-dark: #00b253;
      --blue-light: #2fcbff;
      --blue-dark: #2f63ff;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f2f2f2;
      padding: 2rem;
    }

    .container {
      max-width: 600px;
      margin: auto;
      background: #ffffff;
      padding: 2rem;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      margin-bottom: 1.5rem;
      color: var(--blue-dark);
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    input, select {
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    button {
      padding: 0.75rem;
      background: var(--green-dark);
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background: var(--green-light);
    }

    /* Responsive cho điện thoại */
    @media (max-width: 414px) {
      input, select, button, label {
        font-size: 14px;
      }
    }
    @media (min-width: 415px) and (max-width: 1024px) {
  .container {
    max-width: 80%;
  }
}

/* Responsive cho máy tính */
@media (min-width: 1025px) {
  .container {
    max-width: 600px;
  }
}
  </style>
</head>
<body>

<div class="container">
  <h2>Form Đăng Ký Khóa Học</h2>
  <form id="regForm">
    <label>Họ và tên
      <input type="text" id="fullname" required>
    </label>
    <label>Địa chỉ email
      <input type="email" id="email" required>
    </label>
    <label>Số điện thoại
      <input type="tel" id="phone" required pattern="\d{9,11}">
    </label>
    <label>Khóa học muốn đăng ký
      <select id="course" required>
        <option value="">--Chọn khóa học--</option>
        <option value="Basic English">Basic English</option>
        <option value="Intermediate Conversation">Intermediate Conversation</option>
        <option value="IELTS Intensive">IELTS Intensive</option>
        <option value="Business English">Business English</option>
      </select>
    </label>
    <label>Thời gian ưu tiên học
      <input type="time" id="preftime" required>
    </label>
    <button type="submit">Gửi đăng ký</button>
  </form>
</div>

<script>
  document.getElementById('regForm').addEventListener('submit', function(e){
    e.preventDefault();
    const name = document.getElementById('fullname').value.trim();
    const email = document.getElementById('email').value.trim();
    const phone = document.getElementById('phone').value.trim();
    if(!name || !email || !phone){
      alert('Vui lòng điền đầy đủ thông tin!');
      return;
    }
    if(!/^\d{9,11}$/.test(phone)){
      alert('Số điện thoại phải từ 9–11 chữ số');
      return;
    }
    alert('Đăng ký thành công! Chúng tôi sẽ liên hệ với bạn sớm.');
    this.reset();
  });
</script>

</body>
</html>

Cau 5: 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>English Learning</title>
  <style>
    :root {
      --yellow: #ffe700;
      --green-light: #00e56b;
      --green-dark: #00b253;
      --blue-light: #2fcbff;
      --blue-dark: #2f63ff;
      --item-size: 220px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      padding: 0;
      margin: 0;
      background-color: #f9f9f9;
    }

    header {
      background: var(--blue-dark);
      color: white;
      padding: 1rem 2rem;
      display: flex;
      align-items: center;
      gap: 1rem;
      flex-wrap: wrap;
      flex-direction: column;
      text-align: center;
    }

    header svg {
      width: 48px;
      height: 48px;
      flex-shrink: 0;
    }

    .slogan {
      width: 100%;
      text-align: center;
      font-size: 1.2rem;
      font-style: italic;
      margin: 0.5rem 0;
      color: var(--blue-dark);
    }

    nav {
      background: var(--blue-light);
      width: 100%;
    }

    nav ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      padding: 1rem 2rem;
      justify-content: center;
    }

    nav a {
      color: #000;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      color: white;
    }

    .container {
      max-width: 960px;
      margin: auto;
      padding: 1.5rem;
    }

    .advert {
      width: 100%;
      height: 200px;
      background: var(--yellow);
      border: 2px solid var(--blue-dark);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.2rem;
      text-align: center;
      margin-bottom: 2rem;
      border-radius: 12px;
      transition: 0.3s ease;
    }

    .advert:hover {
      background: var(--green-light);
      border-color: var(--green-dark);
      font-style: italic;
    }

    .items-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin-bottom: 2rem;
    }

    .item {
  width: var(--item-size);
  height: var(--item-size);
  background: var(--blue-light);
  padding: 1rem;
  border-radius: 12px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-shrink: 0; 
}
    .item:hover {
  transform: translateY(-5px);
  transition: 0.3s;
}

    form {
      background: #fff;
      padding: 1.5rem;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    form label {
      display: block;
      margin-top: 1rem;
    }

    form input, form select {
      width: 100%;
      padding: 0.5rem;
      margin-top: 0.3rem;
      border: 1px solid #ccc;
      border-radius: 6px;
    }

    form button {
      margin-top: 1rem;
      padding: 0.5rem 1rem;
      background: var(--green-dark);
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }

    form button:hover {
      background: var(--green-light);
    }

    /* Responsive */
    @media (max-width: 414px) {
      .item {
        width: 100%;
        height: auto;
      }

      nav ul {
        flex-direction: column;
      }

      form {
        padding: 1rem;
      }
    }

    @media (min-width: 1024px) {
  .items-container {
    justify-content: center;
    flex-wrap: nowrap;
  }
}
  </style>
</head>
<body>

  <header>
    <!-- SVG Logo -->
    <svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" aria-label="English Learning Logo">
        <circle cx="32" cy="32" r="32" fill="#2fcbff"/>
        <text x="32" y="38" font-size="28" text-anchor="middle" fill="#2f63ff" font-family="Arial" font-weight="bold">EL</text>
      </svg>
    <h1>English Learning</h1>
  </header>

  <div class="slogan">Learn English, open your world!</div>

  <nav>
    <ul>
      <li><a href="cau1.html">Trang chủ</a></li>
      <li><a href="cau2.html">Quảng cáo</a></li>
      <li><a href="cau3.html">Khóa học</a></li>
      <li><a href="cau4.html">Đăng ký</a></li>
    </ul>
  </nav>

  <div class="container">
    <section class="advert">
      Ưu đãi lớn cho các học viên đăng ký trong tháng này! Giảm đến 50% học phí.
    </section>

    <section>
      <h2 style="text-align:center; margin-bottom: 1rem;">Danh sách khóa học</h2>
      <div class="items-container" id="courseList"></div>
    </section>

    <section>
      <h2 style="text-align:center; margin-bottom: 1rem;">Đăng ký khóa học</h2>
      <form id="registerForm">
        <label>Họ và tên:
          <input type="text" id="name" required>
        </label>
        <label>Địa chỉ email:
          <input type="email" id="email" required>
        </label>
        <label>Số điện thoại:
          <input type="tel" id="phone" required>
        </label>
        <label>Khóa học muốn đăng ký:
          <select id="course" required>
            <option value="">--Chọn khóa học--</option>
        <option value="Basic English">Basic English</option>
        <option value="Intermediate Conversation">Intermediate Conversation</option>
        <option value="IELTS Intensive">IELTS Intensive</option>
        <option value="Business English">Business English</option>
          </select>
        </label>
        <label>Thời gian ưu tiên học:
          <input type="time" id="preftime" required>
        </label>
        <button type="submit">Đăng ký</button>
      </form>
    </section>
  </div>

  <script>
    // JSON data
    const courses = [
    {
    "name": "Basic English",
    "description": "Xây dựng nền tảng từ vựng và ngữ pháp cơ bản.",
    "fee": "3,000,000 VND",
    "start": "2025-06-01"
  },
  {
    "name": "Intermediate Conversation",
    "description": "Nâng cao kỹ năng giao tiếp, phản xạ nhanh.",
    "fee": "4,500,000 VND",
    "start": "2025-06-15"
  },
  {
    "name": "IELTS Intensive",
    "description": "Chuẩn bị IELTS trong 3 tháng với giáo viên bản ngữ.",
    "fee": "8,000,000 VND",
    "start": "2025-07-01"
  },
  {
    "name": "Business English",
    "description": "Kỹ năng tiếng Anh thương mại chuyên sâu.",
    "fee": "6,500,000 VND",
    "start": "2025-07-10"
  }
    ];

    // Hiển thị bằng while loop
    let i = 0;
    const container = document.getElementById('courseList');
    while (i < courses.length) {
      const c = courses[i];
      const div = document.createElement('div');
      div.className = "item";
      div.innerHTML = `<h3>${c.name}</h3>
        <p>${c.description}</p>
        <strong>Học phí: ${c.fee}</strong><br>
        <small>Khai giảng: ${c.start}</small>`;
      container.appendChild(div);
      i++;
    }

    // Form validation
    document.getElementById("registerForm").addEventListener("submit", function(e) {
      const name = document.getElementById("name").value.trim();
      const email = document.getElementById("email").value.trim();
      const phone = document.getElementById("phone").value.trim();
      const course = document.getElementById("course").value;
      const time = document.getElementById("time").value.trim();

      if (!name || !email || !phone || !course || !time) {
        alert("Vui lòng điền đầy đủ thông tin!");
        e.preventDefault();
      }
    });
  </script>
</body>
</html>


![image](https://github.com/user-attachments/assets/f2bc7aa9-7215-4000-a91c-faa74e53960c)
