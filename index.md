## Susie的主页

### 关于我

### 技能

### 联系
- GitHub: [Susie-Yaoyi](https://github.com/Susie-Yaoyi)
- Email: Susie070106@qq.com

<style>
/* 基础样式 */
body {
    background: #fefefe;
    color: #333;
    font-family: 'Segoe UI', system-ui, sans-serif;
    margin: 0;
    padding: 20px;
    min-height: 100vh;
    position: relative;
    overflow-x: hidden;
}

/* 光晕元素 */
.glow {
    position: fixed;
    border-radius: 50%;
    filter: blur(40px);
    opacity: 0.6;
    animation: float 15s infinite ease-in-out;
    z-index: -1;
}

/* 粉色光晕 */
.glow:nth-child(1) {
    width: 300px;
    height: 300px;
    background: rgba(255, 182, 193, 0.4); /* 浅粉色 */
    top: 10%;
    left: 5%;
    animation-delay: 0s;
}

/* 蓝色光晕 */
.glow:nth-child(2) {
    width: 400px;
    height: 400px;
    background: rgba(173, 216, 230, 0.3); /* 浅蓝色 */
    bottom: 5%;
    right: 10%;
    animation-delay: -5s;
}

/* 薄荷绿光晕 */
.glow:nth-child(3) {
    width: 250px;
    height: 250px;
    background: rgba(152, 251, 152, 0.25); /* 浅绿色 */
    top: 50%;
    left: 70%;
    animation-delay: -10s;
}

/* 光晕浮动动画 */
@keyframes float {
    0%, 100% {
        transform: translate(0, 0) scale(1);
    }
    25% {
        transform: translate(20px, 20px) scale(1.1);
    }
    50% {
        transform: translate(-15px, 15px) scale(0.9);
    }
    75% {
        transform: translate(10px, -10px) scale(1.05);
    }
}

/* 内容容器 */
.container {
    max-width: 800px;
    margin: 40px auto;
    background: rgba(255, 255, 255, 0.85);
    padding: 40px;
    border-radius: 20px;
    backdrop-filter: blur(10px);
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
    border: 1px solid rgba(255, 255, 255, 0.2);
}

/* 标题样式 */
.header {
    text-align: center;
    margin-bottom: 40px;
}

.name {
    font-size: 2.5em;
    color: #5d8aa8;
    margin-bottom: 10px;
    font-weight: 300;
}

.tagline {
    font-size: 1.2em;
    color: #7f8c8d;
    font-style: italic;
}

/* 卡片样式 */
.card {
    background: rgba(255, 255, 255, 0.9);
    padding: 25px;
    margin: 20px 0;
    border-radius: 15px;
    border-left: 4px solid #a8d8ea;
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
}

/* 技能标签 */
.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 15px;
}

.skill-tag {
    background: linear-gradient(135deg, #a8d8ea, #cce7ff);
    color: #2c3e50;
    padding: 8px 16px;
    border-radius: 20px;
    font-size: 0.9em;
    border: 1px solid rgba(255, 255, 255, 0.5);
}
</style>

<!-- 光晕背景 -->
<div class="glow"></div>
<div class="glow"></div>
<div class="glow"></div>
