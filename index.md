<style>
/* 基础样式 */
body {
    background: #f8f9fa;
    margin: 0;
    padding: 0;
    position: relative;
    overflow-x: hidden;
    font-family: "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
}

/* 简约光晕 - 非常 subtle */
.glow {
    position: fixed;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.3;  /* 很低的不透明度 */
    animation: float 25s infinite ease-in-out;
    z-index: -1;
}

.glow:nth-child(1) {
    width: 200px;
    height: 200px;
    background: rgba(180, 220, 255, 0.2);  /* 非常淡的蓝色 */
    top: 20%;
    left: 10%;
    animation-delay: 0s;
}

.glow:nth-child(2) {
    width: 150px;
    height: 150px;
    background: rgba(255, 200, 220, 0.15); /* 非常淡的粉色 */
    bottom: 30%;
    right: 15%;
    animation-delay: -8s;
}

.glow:nth-child(3) {
    width: 180px;
    height: 180px;
    background: rgba(200, 255, 220, 0.1);  /* 几乎看不见的绿色 */
    top: 60%;
    left: 80%;
    animation-delay: -15s;
}

/* 非常缓慢的浮动 */
@keyframes float {
    0%, 100% { 
        transform: translate(0, 0) scale(1); 
    }
    25% { 
        transform: translate(10px, 15px) scale(1.02); 
    }
    50% { 
        transform: translate(-8px, 10px) scale(0.98); 
    }
    75% { 
        transform: translate(5px, -8px) scale(1.01); 
    }
}

/* Cayman 风格页面头部 */
.page-header {
    color: #fff;
    text-align: center;
    background-color: #159957;
    background-image: linear-gradient(120deg, #155799, #159957);
    padding: 5rem 6rem;
    position: relative;
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
    background: rgba(255, 255, 255, 0.95); /* 更实心的背景 */
}

@media screen and (max-width: 42em) {
    .page-header {
        padding: 3rem 1rem;
    }
    .project-name {
        font-size: 2.25rem;
    }
    .project-tagline {
        font-size: 1.2rem;
    }
    .main-content {
        padding: 2rem 1rem;
        font-size: 1rem;
    }
}

/* 简约卡片 */
.card {
    background: white;
    padding: 1.5rem;
    margin: 1.5rem 0;
    border-radius: 8px;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
    border-left: 3px solid #159957;
    transition: all 0.2s ease;
}

.card:hover {
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

/* 简约技能标签 */
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

<!-- 简约光晕背景 -->
<div class="glow"></div>
<div class="glow"></div>
<div class="glow"></div>

<!-- Cayman 风格页面头部 -->
<header class="page-header">
    <h1 class="project-name">Susie's Space</h1>
    <h2 class="project-tagline">简约而不简单，细节中见品味</h2>
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
            <span class="skill-tag">（）</span>
            <span class="skill-tag">（）</span>
            <span class="skill-tag">（）</span>
        </div>
    </div>
    
    <div class="card">
        <h2>📬 联系</h2>
        <p>📧 Susie070106@qq.com<br>
           💼 GitHub: @Susie-Yaoyi</p >
    </div>
</main>
