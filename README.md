/*
 * Clash Verge Rev 主题 CSS 注入
 * 用途：自定义节点延迟指示器（the-delay）的颜色映射，将其与主题状态色绑定。
 * 使用方法：复制全部内容，粘贴到 Clash-Verge-Rev → 主题设置 → CSS注入 → CSS编辑器，保存即可。
 */

/*
 * 状态映射：error.main（错误 / 超时）
 * 将延迟显示为 error.main 状态的元素强制改为红色。
 * 对应通常的“超时”或“连接失败”等异常状态。
 */
div.the-delay[color="error.main"] {
  color: #ff4d4f !important; /* 自定义错误状态颜色，默认浅红色，可自行替换为喜欢的红色 HEX 色值 */
}

/*
 * 状态映射：warning.main（警告 / 较高延迟）
 * 将原本可能显示为蓝色或其他颜色的 warning.main 状态强制改为黄色（警告色）。
 * 这样在视觉上更符合直觉：高延迟用黄色突出显示。
 */
div.the-delay[color="warning.main"] {
  color: #faad14 !important; /* 强制修改为黄色，用于表示较高延迟的警告状态 */
}

/*
 * 状态映射：success.main（成功 / 低延迟）
 * 将延迟显示为 success.main 状态的元素强制改为绿色。
 * 表示延迟较低，连接质量良好。
 */
div.the-delay[color="success.main"] {
  color: #52c41a !important; /* 绿色，表示正常 / 低延迟 */
}

/*
 * 状态映射：primary.main（主要 / 一般延迟）
 * 将延迟显示为 primary.main 状态的元素强制改为蓝色。
 * 一般用于中等延迟或默认主题强调色。
 */
div.the-delay[color="primary.main"] {
  color: #1976d2 !important; /* 蓝色，表示普通或中等延迟 */
}
