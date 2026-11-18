# Animation Performance CN

**先查明为什么掉帧，再决定怎么改。**

## 功能与流程

保留帧预算、布局/绘制/合成成本、主线程、React逐帧更新、继承CSS变量、模糊效果和 will-change 的原始诊断方法。先列出动画与驱动，再按原因排查，以代码和设备录制区分推断与实测。

中文补充帮助把“卡顿、不跟手、内容多了变慢”对应到排查场景，并标明“代码已确认、录制已确认、仍需验证”。不修改原技术规则，不宣称自动保证流畅。

## 安装与调用

```bash
npx skills add batespaige357-tech/animation-performance-cn --skill animation-performance-cn
```

对助手说：“用 animation-performance-cn 排查这个网页动画为什么掉帧，先诊断，标明哪些需要设备录制。”Codex 可使用 `$animation-performance-cn`。手动安装可复制 `skills/animation-performance-cn` 完整目录。

适用于网页动画性能；不负责选择动画风格、缓动或是否应该添加动画，也不覆盖 React Native 线程诊断。相关主题可查看上游 animate、review-animations、animate-expo，本包不捆绑这些技能。真实测量需要项目、浏览器工具和目标设备，本包不包含分析器。

## 来源与许可

基于 [emilkowalski/skills 的 animation-performance](https://github.com/emilkowalski/skills/tree/main/skills/animation-performance)，由本仓库维护。

MIT，保留 Emil Kowalski 原版权与完整许可证；具体改动见 [CHANGES.md](CHANGES.md)。开场白已中文化，移除虚构个人项目经历的角色表述，核心诊断正文保留。

已检查正文差异、UTF-8、本地引用和技能格式；未运行真实动画、性能录制、设备测试或助手行为评估。未运行前端编译，不含示例网页、效果截图或前后对比。
