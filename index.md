<style>
/* 基础样式 */
body {
    background: #fafbfc;
    margin: 0;
    padding: 0;
    position: relative;
    overflow-x: hidden;
    font-family: "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
}

/* 光晕效果 */
.glow {
    position: fixed;
    border-radius: 50%;
    filter: blur(70px);
    opacity: 0.4;
    animation: float 20s infinite ease-in-out;
    z-index: -1;
    pointer-events: none;
}

.glow:nth-child(1) {
    width: 250px;
    height: 250px;
    background: rgba(180, 220, 255, 0.3);
    top: 15%;
    left: 8%;
    animation-delay: 0s;
}

.glow:nth-child(2) {
    width: 200px;
    height: 200px;
    background: rgba(255, 200, 220, 0.25);
    bottom: 25%;
    right: 12%;
    animation-delay: -7s;
}

.glow:nth-child(3) {
    width: 220px;
    height: 220px;
    background: rgba(200, 255, 220, 0.2);
    top: 55%;
    left: 75%;
    animation-delay: -12s;
}

/* 浮动动画 */
@keyframes float {
    0%, 100% { 
        transform: translate(0, 0) scale(1); 
    }
    33% { 
        transform: translate(15px, 20px) scale(1.05); 
    }
    66% { 
        transform: translate(-10px, 15px) scale(0.95); 
    }
}

/* 页面头部 */
.page-header {
    color: #fff;
    text-align: center;
    background-color: #159957;
    background-image: linear-gradient(120deg, #155799, #159957);
    padding: 5rem 6rem;
}

.project-name {
    margin-top: 0;
    margin-bottom: 0.1rem;
    font-size: 3.25rem;
    font-weight: 300;
}

.project-tagline {
    margin-bottom: 2rem;
    font-weight: 300;
    opacity: 0.9;
    font-size: 1.5rem;
}

/* 主内容区域 */
.main-content {
    max-width: 64rem;
    padding: 2rem 6rem;
    margin: 0 auto;
    font-size: 1.1rem;
    background: rgba(255, 255, 255, 0.95);
}

.card {
    background: white;
    padding: 1.5rem;
    margin: 1.5rem 0;
    border-radius: 8px;
    box-shadow: 0 2px 6px rgba(0, 0, 0, 0.04);
    border-left: 3px solid #159957;
}

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 1rem;
}

.skill-tag {
    background: #f8f9fa;
    color: #159957;
    padding: 0.3rem 0.8rem;
    border-radius: 12px;
    font-size: 0.9rem;
    border: 1px solid #e9ecef;
}
</style>

<!-- 光晕背景 -->
<div class="glow"></div>
<div class="glow"></div>
<div class="glow"></div>

<!-- 页面头部 -->
<header class="page-header">
    <h1 class="project-name">Susie's Space</h1>
    <h2 class="project-tagline">欢迎来到我的空间</h2>
</header>

<!-- 主内容区域 -->
<main class="main-content">
    <div class="card">
        <h2>💫 关于我</h2>
        <p>（没想好啦）</p >
    </div>
    
    <div class="card">
        <h2>🛠️ 技能</h2>
        <div class="skills">
            <span class="skill-tag">1</span>
            <span class="skill-tag">2</span>
            <span class="skill-tag">3</span>
        </div>
    </div>
    
    <div class="card">
        <h2>📬 联系</h2>
        <p>📧 Susie070106@qq.com<br>
           💼 GitHub: @Susie-Yaoyi</p >
    </div>
</main>
