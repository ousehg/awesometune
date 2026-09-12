# AwesomeTune

一个单文件网页小应用：简谱速读（随机数字组练音名 / 唱名反应）和音准训练（麦克风实时音准表）。

- 点按 / 键盘作答、唱读自评、念唱名（手机语音识别）、念唱名自训练（用自己的录音做模板，MFCC + DTW 比对）、视唱识音（音高检测）
- 高音点 / 低音点、调号（1=C…B）、每组 4 / 8 / 12 个
- 吉他 / 钢琴 / 合成三种音色，计时、正确率、最佳成绩

只有一个文件 `index.html`，浏览器直接打开即可。视唱识音需要麦克风，必须通过 https 地址访问。

## 部署到 GitHub Pages

1. 在 GitHub 新建一个仓库（`awesometune`），不要勾选初始化 README。
2. 在本目录执行：

   ```bash
   git remote add origin git@github.com:ousehg/awesometune.git
   git push -u origin main
   ```

3. 打开仓库的 Settings → Pages，Source 选 "Deploy from a branch"，Branch 选 `main` / `/ (root)`，保存。
4. 一两分钟后访问 `https://ousehg.github.io/awesometune/`。

以后改了 `index.html`，`git commit` 再 `git push` 即可更新。
