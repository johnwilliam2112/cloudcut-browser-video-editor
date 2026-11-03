CloudCut – Browser Video Editor

Multilingual README: English | 简体中文 | فارسی

---

1. English

CloudCut – Browser Video Editor

CloudCut is a browser-based video editor powered by Cloudflare Workers and FFmpeg.wasm. It provides a mobile-friendly interface and processes media locally in the user's browser.

Features

Video Editing

- Trim and cut video clips
- Merge multiple clips
- Resize and crop
- Rotate and flip
- Change playback speed
- Adjust brightness, contrast, and saturation
- Apply visual effects
- Add text overlays and image watermarks
- Add subtitles

Audio Editing

- Remove or replace audio
- Mix audio tracks
- Normalize audio
- Add fade-in and fade-out
- Export audio separately

Supported Media Formats

- Video: MP4, WebM, MKV
- Audio: MP3, WAV
- Animation: GIF
- Images: JPG
- Subtitles: SRT, ASS, SSA, VTT

Actual format and codec support depends on the FFmpeg.wasm build and browser.

Export Presets

- YouTube 1080p
- Vertical video (9:16)
- Smaller file size
- GIF
- MP3 audio

Other Features

- Mobile-friendly interface
- Multiple media selection
- English, Persian, and Chinese interface options
- Browser-side media processing
- No server-side video storage

Deploy to Cloudflare

""Deploy to Cloudflare" (https://deploy.workers.cloudflare.com/button)" (https://deploy.workers.cloudflare.com/?url=https://github.com/johnwilliam2112/cloudcut-browser-video-editor)

1. Select Deploy to Cloudflare.
2. Sign in to your Cloudflare account.
3. Connect your GitHub account if requested.
4. Review the Worker configuration.
5. Deploy the project.

Each deployment creates an independent Worker for its owner.

Manual Installation

Cloudflare Dashboard

1. Open https://dash.cloudflare.com/
2. Go to Workers & Pages.
3. Create a new Worker.
4. Open the code editor.
5. Copy the contents of "worker.js" into the editor.
6. Save and deploy.

Wrangler CLI

Clone the repository:

git clone https://github.com/johnwilliam2112/cloudcut-browser-video-editor.git
cd cloudcut-browser-video-editor

Example "wrangler.jsonc":

{
  "name": "cloudcut-browser-video-editor",
  "main": "worker.js",
  "compatibility_date": "2026-11-02"
}

Deploy:

npx wrangler deploy

Technology

- Cloudflare Workers
- HTML5, CSS3, and JavaScript
- FFmpeg.wasm
- Browser Web APIs

The project does not require a Node.js server for video processing. The Worker serves the web application; media processing takes place in the browser.

Privacy

Selected media is processed locally in the browser and is not uploaded to the Worker for processing. The Worker serves the application. FFmpeg.wasm and its runtime assets may be loaded from external CDNs.

Requirements and Limitations

- Use a modern browser.
- An internet connection is required to load external FFmpeg assets.
- Large videos can require substantial device memory.
- Processing speed depends on the device and browser.
- Codec support depends on the FFmpeg.wasm build.
- Keep the browser tab open while processing.

Repository

https://github.com/johnwilliam2112/cloudcut-browser-video-editor

Typical project files:

- "worker.js" — Cloudflare Worker and web application
- "wrangler.jsonc" — Wrangler configuration
- "README.md" — Project documentation

License

No license is specified here. Unless a license is added to the repository, all rights remain with the copyright holder.

---

2. 简体中文

CloudCut – 浏览器视频编辑器

CloudCut 是一款基于浏览器的视频编辑器，使用 Cloudflare Workers 和 FFmpeg.wasm。它提供适合手机使用的界面，并在用户的浏览器本地处理媒体文件。

功能

视频编辑

- 修剪和剪切视频片段
- 合并多个视频片段
- 调整尺寸和裁剪
- 旋转和翻转
- 调整播放速度
- 调整亮度、对比度和饱和度
- 应用视觉效果
- 添加文字和图片水印
- 添加字幕

音频编辑

- 移除或替换音频
- 混合多个音轨
- 音量标准化
- 添加淡入和淡出效果
- 单独导出音频

支持的媒体格式

- 视频：MP4、WebM、MKV
- 音频：MP3、WAV
- 动画：GIF
- 图片：JPG
- 字幕：SRT、ASS、SSA、VTT

实际支持的格式和编解码器取决于 FFmpeg.wasm 构建版本和浏览器。

导出预设

- YouTube 1080p
- 竖屏视频（9:16）
- 较小的文件体积
- GIF
- MP3 音频

其他功能

- 适合手机使用的界面
- 支持选择多个媒体文件
- 支持英语、波斯语和中文界面
- 在浏览器本地处理媒体
- 不在服务器端存储视频

部署到 Cloudflare

""Deploy to Cloudflare" (https://deploy.workers.cloudflare.com/button)" (https://deploy.workers.cloudflare.com/?url=https://github.com/johnwilliam2112/cloudcut-browser-video-editor)

1. 点击 Deploy to Cloudflare。
2. 登录 Cloudflare 账户。
3. 如有提示，请连接 GitHub 账户。
4. 检查 Worker 配置。
5. 部署项目。

每次部署都会为部署者创建一个独立的 Worker。

手动安装

使用 Cloudflare Dashboard

1. 打开 https://dash.cloudflare.com/
2. 进入 Workers & Pages。
3. 创建一个新的 Worker。
4. 打开代码编辑器。
5. 将 "worker.js" 的内容复制到编辑器中。
6. 保存并部署。

使用 Wrangler CLI

克隆项目仓库：

git clone https://github.com/johnwilliam2112/cloudcut-browser-video-editor.git
cd cloudcut-browser-video-editor

示例 "wrangler.jsonc"：

{
  "name": "cloudcut-browser-video-editor",
  "main": "worker.js",
  "compatibility_date": "2026-11-02"
}

部署：

npx wrangler deploy

技术

- Cloudflare Workers
- HTML5、CSS3 和 JavaScript
- FFmpeg.wasm
- 浏览器 Web API

视频处理不需要 Node.js 服务器。Worker 负责提供网页应用，媒体处理在浏览器中完成。

隐私

所选媒体文件在浏览器本地处理，不会为了处理而上传到 Worker。Worker 负责提供应用程序。FFmpeg.wasm 及其运行时资源可能从外部 CDN 加载。

系统要求与限制

- 请使用现代浏览器。
- 加载外部 FFmpeg 资源需要互联网连接。
- 大型视频可能需要较多设备内存。
- 处理速度取决于设备和浏览器。
- 编解码器支持取决于 FFmpeg.wasm 构建版本。
- 处理期间请保持浏览器标签页打开。

项目仓库

https://github.com/johnwilliam2112/cloudcut-browser-video-editor

常见项目文件：

- "worker.js" — Cloudflare Worker 和网页应用
- "wrangler.jsonc" — Wrangler 配置
- "README.md" — 项目说明文档

许可证

此处未指定许可证。除非仓库中添加了许可证，否则所有权利仍归版权持有人所有。

---

3. فارسی

CloudCut – ویرایشگر ویدئوی تحت وب

CloudCut یک ویرایشگر ویدئو تحت وب است که با Cloudflare Workers و FFmpeg.wasm کار می‌کند. این برنامه رابطی سازگار با موبایل دارد و فایل‌های رسانه‌ای را به‌صورت محلی در مرورگر کاربر پردازش می‌کند.

امکانات

ویرایش ویدئو

- کوتاه‌کردن و برش کلیپ‌ها
- ادغام چند کلیپ
- تغییر اندازه و برش تصویر
- چرخاندن و معکوس‌کردن ویدئو
- تغییر سرعت پخش
- تنظیم روشنایی، کنتراست و اشباع رنگ
- اعمال جلوه‌های تصویری
- افزودن متن و واترمارک تصویری
- افزودن زیرنویس

ویرایش صدا

- حذف یا جایگزینی صدا
- ترکیب چند ترک صوتی
- یکسان‌سازی سطح صدا
- افزودن محوشدن تدریجی صدا در ابتدا و انتها
- خروجی گرفتن جداگانه از صدا

قالب‌های رسانه‌ای پشتیبانی‌شده

- ویدئو: MP4، WebM، MKV
- صدا: MP3، WAV
- انیمیشن: GIF
- تصویر: JPG
- زیرنویس: SRT، ASS، SSA، VTT

پشتیبانی واقعی از قالب‌ها و کدک‌ها به نسخه ساخت FFmpeg.wasm و مرورگر بستگی دارد.

تنظیمات آماده خروجی

- YouTube 1080p
- ویدئوی عمودی (9:16)
- حجم فایل کمتر
- GIF
- صدای MP3

امکانات دیگر

- رابط کاربری سازگار با موبایل
- انتخاب چند فایل رسانه‌ای
- رابط کاربری انگلیسی، فارسی و چینی
- پردازش رسانه در مرورگر
- بدون ذخیره ویدئو روی سرور

استقرار روی Cloudflare

""Deploy to Cloudflare" (https://deploy.workers.cloudflare.com/button)" (https://deploy.workers.cloudflare.com/?url=https://github.com/johnwilliam2112/cloudcut-browser-video-editor)

1. روی Deploy to Cloudflare کلیک کنید.
2. وارد حساب Cloudflare خود شوید.
3. در صورت درخواست، حساب GitHub خود را متصل کنید.
4. تنظیمات Worker را بررسی کنید.
5. پروژه را Deploy کنید.

هر بار استقرار، یک Worker مستقل برای مالک آن ایجاد می‌کند.

نصب دستی

از طریق Cloudflare Dashboard

1. وارد https://dash.cloudflare.com/ شوید.
2. به بخش Workers & Pages بروید.
3. یک Worker جدید ایجاد کنید.
4. ویرایشگر کد را باز کنید.
5. محتوای فایل "worker.js" را در ویرایشگر قرار دهید.
6. فایل را ذخیره و Deploy کنید.

از طریق Wrangler CLI

مخزن پروژه را دریافت کنید:

git clone https://github.com/johnwilliam2112/cloudcut-browser-video-editor.git
cd cloudcut-browser-video-editor

نمونه فایل "wrangler.jsonc":

{
  "name": "cloudcut-browser-video-editor",
  "main": "worker.js",
  "compatibility_date": "2026-11-02"
}

استقرار:

npx wrangler deploy

فناوری‌ها

- Cloudflare Workers
- HTML5، CSS3 و JavaScript
- FFmpeg.wasm
- Web APIهای مرورگر

برای پردازش ویدئو به سرور Node.js نیازی نیست. Worker برنامه وب را ارائه می‌کند و پردازش رسانه در مرورگر انجام می‌شود.

حریم خصوصی

فایل‌های انتخاب‌شده برای پردازش به Worker آپلود نمی‌شوند و به‌صورت محلی در مرورگر پردازش می‌شوند. Worker فقط برنامه را ارائه می‌کند. فایل‌های FFmpeg.wasm و منابع اجرایی آن ممکن است از CDNهای خارجی بارگذاری شوند.

پیش‌نیازها و محدودیت‌ها

- از یک مرورگر به‌روز استفاده کنید.
- برای بارگذاری منابع خارجی FFmpeg به اینترنت نیاز است.
- ویدئوهای حجیم ممکن است به حافظه زیادی نیاز داشته باشند.
- سرعت پردازش به دستگاه و مرورگر بستگی دارد.
- پشتیبانی از کدک‌ها به نسخه ساخت FFmpeg.wasm وابسته است.
- هنگام پردازش، زبانه مرورگر را باز نگه دارید.

مخزن پروژه

https://github.com/johnwilliam2112/cloudcut-browser-video-editor

فایل‌های اصلی پروژه:

- "worker.js" — کد Cloudflare Worker و برنامه وب
- "wrangler.jsonc" — تنظیمات Wrangler
- "README.md" — مستندات پروژه

مجوز

در این مستند مجوزی مشخص نشده است. تا زمانی که مجوزی به مخزن اضافه نشود، تمام حقوق برای دارنده حق نشر محفوظ است.
