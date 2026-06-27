# chenjie
<!doctype html>
<html lang="zh-CN">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="微光" />
  <title>毕业礼物</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <a class="logo" href="#">
        <!-- Inline SVG logo -->
        <svg width="36" height="36" viewBox="0 0 24 24" fill="none" aria-hidden="true">
          <rect x="2" y="2" width="20" height="20" rx="5" fill="var(--accent)"/>
          <path d="M7 12h10" stroke="white" stroke-width="1.5" stroke-linecap="round"/>
          <path d="M7 16h6" stroke="white" stroke-width="1.5" stroke-linecap="round"/>
        </svg>
        <span>产品名</span>
      </a>

      <nav class="nav" id="nav">
        <a href="#features">功能</a>
        <a href="#about">关于</a>
        <a href="#contact">联系</a>
        <a class="btn-outline" href="#contact">立即咨询</a>
      </nav>

      <button class="nav-toggle" id="navToggle" aria-label="打开菜单">☰</button>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-inner">
        <div class="hero-content">
          <h1>不要忘记我</h1>
          <p class="lede">一个简洁的落地页模板，响应式、易扩展，并支持表单提交到 Formspree 或你自己的后端。</p>
          <div class="hero-cta">
            <a class="btn" href="#contact">免费咨询</a>
            <a class="btn-ghost" href="#features">了解更多</a>
          </div>
        </div>
        <div class="hero-art">
          <img alt="示例图" src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='480' height='320'><rect fill='%23f3f4f6' width='100%25' height='100%25'/><text x='50%25' y='50%25' dominant-baseline='middle' text-anchor='middle' fill='%23888' font-size='20'>示例图片占位</text></svg>">
        </div>
      </div>
    </section>

    <section id="features" class="container features">
      <h2>核心功能</h2>
      <div class="grid">
        <div class="card">
          <h3>响应式设计</h3>
          <p>在手机、平板与桌面上都能良好展示，无需额外设置。</p>
        </div>
        <div class="card">
          <h3>快速部署</h3>
          <p>支持 GitHub Pages / Netlify / Vercel 等一键部署方案。</p>
        </div>
        <div class="card">
          <h3>联系表单</h3>
          <p>表单可提交到 Formspree，也可以接入你的后端 API。</p>
        </div>
      </div>
    </section>

    <section id="about" class="about container">
      <h2>关于我们</h2>
      <p>我们专注于为中小型团队和个人提供简洁、高效的网站解决方案。你可以根据需要修改文案、颜色和图片。</p>
    </section>

    <section id="contact" class="contact container">
      <h2>联系我们</h2>
      <p>填写下方表单，但是老子懒得回。</p>

      <!-- 注意：将 action 替换为你的 Formspree ID 或后端 API -->
      <form id="contactForm" action="https://formspree.io/f/your-form-id" method="POST" class="form">
        <label>
          名称
          <input type="text" name="name" required placeholder="你的姓名" />
        </label>
        <label>
          邮箱
          <input type="email" name="email" required placeholder="name@example.com" />
        </label>
        <label>
          信息
          <textarea name="message" rows="5" required placeholder="请输入你的需求或问题"></textarea>
        </label>
        <button class="btn" type="submit">发送消息</button>
        <p id="formMsg" class="form-msg" role="status" aria-live="polite"></p>
      </form>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container">
      <p>© <span id="year"></span> 产品名。版权所有。</p>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>
