# B-tech
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bushra Tech</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #f1f4ff;
            color: #000;
            line-height: 1.7;
        }

        /* HEADER */
        header {
            background: #0b4fff;
            color: white;
            padding: 60px 20px;
            text-align: center;
        }

            header img {
                width: 150px;
                border-radius: 10px;
                margin-bottom: 15px;
            }

            header h1 {
                margin: 0;
                font-size: 50px;
                font-weight: bold;
                letter-spacing: 2px;
            }

        /* ABOUT SECTION */
        .about {
            max-width: 900px;
            margin: 50px auto;
            text-align: center;
            padding: 20px;
        }

            .about h2 {
                font-size: 34px;
                margin-bottom: 15px;
            }

            .about p {
                font-size: 20px;
                color: #333;
            }

        /* SERVICE CARDS */
        .services-container {
            max-width: 1100px;
            margin: 30px auto;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 25px;
        }

        .service-card {
            background: white;
            width: 260px;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0px 4px 20px rgba(0,0,0,0.1);
            text-align: center;
        }

            .service-card h3 {
                margin-top: 0;
                font-size: 22px;
            }

            .service-card p {
                margin: 10px 0;
                color: #444;
            }

            .service-card button {
                margin-top: 10px;
                background: #0b4fff;
                color: white;
                border: none;
                padding: 12px 20px;
                border-radius: 8px;
                cursor: pointer;
                font-size: 17px;
            }

        /* POPUP FORM */
        .popup {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.5);
            justify-content: center;
            align-items: center;
        }

        .popup-box {
            background: white;
            padding: 25px;
            width: 330px;
            border-radius: 10px;
            text-align: center;
        }

            .popup-box input, .popup-box textarea {
                width: 90%;
                padding: 12px;
                margin: 8px 0;
                border: 1px solid #ccc;
                border-radius: 8px;
            }

            .popup-box button {
                width: 100%;
                background: #0b4fff;
                color: white;
                padding: 14px;
                border: none;
                border-radius: 8px;
                cursor: pointer;
                font-size: 18px;
            }

        /* CONTACT SECTION */
        .contact {
            max-width: 900px;
            margin: 40px auto;
            text-align: center;
            padding: 20px;
        }

            .contact h3 {
                font-size: 30px;
                margin-bottom: 10px;
            }

            .contact p {
                font-size: 18px;
                color: #222;
            }

        /* FOOTER */
        footer {
            background: #0b4fff;
            color: white;
            padding: 20px;
            text-align: center;
            margin-top: 40px;
            font-size: 16px;
        }
    </style>

</head>

<body>

    <!-- HEADER -->
    <header>
        <img src="https://i.postimg.cc/B6KC4Q4Q/2D10377C-4CE1-4539-92E8-45C1E7752386.jpg" alt="Bushra Tech Logo">
        <h1>Bushra Tech</h1>
    </header>

    <!-- ABOUT -->
    <div class="about">
        <h2>حلول تقنية متطورة لشغلك في مكان واحد</h2>
        <p>
            بشرة تك بتقدم خدمات رقمية كاملة بجودة عالية وشكل احترافي يناسب المشاريع اللي
            عايزة تطور حضورها الرقمي وتكبر قدام جمهورها.
            بنوفر تصميم مواقع حديثة، وشات بوت ذكي، وأنظمة صوتية بالذكاء الاصطناعي،
            وتصميم لوجوهات احترافية، وتطوير تطبيقات بسيطة وسريعة الاستخدام.
            فريقنا بيشتغل معاك خطوة بخطوة لحد ما نوصل لأفضل نتيجة،
            ونخلي شغلك شكله قوي وواضح قدام العملاء والمنافسين.
            بنهتم بالسرعة، الجودة، وسهولة التواصل — كل حاجة بتتم بشكل بسيط ومنظم.
        </p>
    </div>

    <!-- SERVICES -->
    <div class="services-container">

        <div class="service-card">
            <h3>موقع إلكتروني</h3>
            <p>موقع كامل حديث واحترافي.</p>
            <p><strong>٨٠٠٠ جنيه</strong></p>
            <button onclick="openPopup('موقع إلكتروني (٨٠٠٠ جنيه)')">اطلب الآن</button>
        </div>

        <div class="service-card">
            <h3>شات بوت AI</h3>
            <p>روبوت ذكي للرد على العملاء تلقائيًا.</p>
            <p><strong>٤٠٠٠ جنيه</strong></p>
            <button onclick="openPopup('شات بوت AI (٤٠٠٠ جنيه)')">اطلب الآن</button>
        </div>

        <div class="service-card">
            <h3>نظام صوتي AI</h3>
            <p>مساعد صوتي تلقائي.</p>
            <p><strong>٣٠٠٠ جنيه</strong></p>
            <button onclick="openPopup('نظام صوتي AI (٣٠٠٠ جنيه)')">اطلب الآن</button>
        </div>

        <div class="service-card">
            <h3>تصميم لوجو</h3>
            <p>هوية بصرية ولوجو محترف.</p>
            <p><strong>١٥٠٠ جنيه</strong></p>
            <button onclick="openPopup('تصميم لوجو (١٥٠٠ جنيه)')">اطلب الآن</button>
        </div>

        <div class="service-card">
            <h3>تطبيق بسيط</h3>
            <p>تطبيق بسيط وسريع حسب طلبك.</p>
            <p><strong>١٥٠٠٠ جنيه</strong></p>
            <button onclick="openPopup('تطبيق بسيط (١٥٠٠٠ جنيه)')">اطلب الآن</button>
        </div>

    </div>


    <!-- CONTACT -->
    <div class="contact">
        <h3>تواصل معنا</h3>
        <p><strong>الإيميل:</strong> support@bushratech.com</p>
        <p><strong>رقم الموبايل:</strong> 12262122075+</p>
        <p><strong>إنستجرام:</strong> @bushratech</p>
        <p><strong>تويتر:</strong> @bushratech</p>
    </div>


    <!-- POPUP FORM -->
    <div class="popup" id="popup">
        <div class="popup-box">
            <h3 id="serviceName"></h3>

            <input id="firstName" placeholder="الاسم الأول">
            <input id="lastName" placeholder="اسم العائلة">
            <input id="phone" placeholder="رقم الموبايل">
            <input id="email" placeholder="الإيميل (اختياري)">
            <textarea id="details" placeholder="تفاصيل المشروع (اختياري)" rows="3"></textarea>

            <button onclick="sendToWhatsApp()">إرسال</button>
        </div>
    </div>

    <!-- FOOTER -->
    <footer>
        © ٢٠٢٥ Bushra Tech — جميع الحقوق محفوظة
    </footer>

    <script>
        let selectedService = "";

        function openPopup(service) {
            selectedService = service;
            document.getElementById("serviceName").innerText = service;
            document.getElementById("popup").style.display = "flex";
        }

        function sendToWhatsApp() {
            const f = document.getElementById("firstName").value;
            const l = document.getElementById("lastName").value;
            const p = document.getElementById("phone").value;
            const e = document.getElementById("email").value;
            const d = document.getElementById("details").value;

            const message =
                "طلب جديد:%0A" +
                "الخدمة: " + selectedService + "%0A" +
                "الاسم الأول: " + f + "%0A" +
                "اسم العائلة: " + l + "%0A" +
                "رقم الموبايل: " + p + "%0A" +
                "الإيميل: " + e + "%0A" +
                "تفاصيل المشروع: " + d;

            window.open("https://wa.me/12262122075?text=" + message);
            document.getElementById("popup").style.display = "none";
        }
    </script>

</body>
</html>
