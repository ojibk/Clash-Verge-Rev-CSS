使用方法：将如下代码复制、粘贴到 Clash-Verge-Rev → 主题设置 → CSS注入 → CSS编辑器里并保存。

/* 映射 "error.main" 状态 */
div.the-delay[color="error.main"] {
color: #ff4d4f !important; /* 你可以修改为你喜欢的红色的 HEX 色值 */
}

/* 状态映射 warning.main */
div.the-delay[color="warning.main"] {
color: #faad14 !important; /* 强制把蓝色的档位改成黄色 */
}

/* 状态映射 success.main */
div.the-delay[color="success.main"] {
color: #52c41a !important;
}

/* 状态映射 primary.main */
div.the-delay[color="primary.main"] {
color: #1976d2 !important;
}
