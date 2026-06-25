<div align="center">
  <!-- 敲代码的动图，跟随系统深色/浅色模式 -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://cdn.jsdelivr.net/gh/sun0225SUN/sun0225SUN/assets/images/coding.gif" />
    <source media="(prefers-color-scheme: light)" srcset="https://cdn.jsdelivr.net/gh/sun0225SUN/sun0225SUN/assets/images/developer.svg" height="225px" />
    <img src="https://cdn.jsdelivr.net/gh/sun0225SUN/sun0225SUN/assets/images/coding.gif" alt="coding" />
  </picture>

  <div>&nbsp;</div>

  <!-- 访问量统计 -->
  <img src="https://komarev.com/ghpvc/?username=34204002&label=来过的人&color=orange&style=flat" alt="profile views" />

  <div>&nbsp;</div>

  <!-- 贪吃蛇贡献图（需要配置 GitHub Action 才会动起来，说明在最底部） -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/34204002/34204002/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/34204002/34204002/output/github-contribution-grid-snake.svg" />
    <img alt="snake eating my contributions" src="https://raw.githubusercontent.com/34204002/34204002/output/github-contribution-grid-snake.svg" />
  </picture>
</div>

---

# 👋 你好，我是 Jiang_I

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=22&pause=1000&color=00BFFF&center=true&vCenter=true&width=450&lines=System.out.println(%22Hello%2C+world%22);while(true)+%7B+keep+building%3B+%7D" alt="Typing SVG" />
</div>

<br>

<table>
<tr>
<td>

### 🧠 关于我

<img align="right" width="100" src="https://avatars.githubusercontent.com/u/34204002?v=4" />

&emsp;&emsp;嗨，我是 Jiang。写 Java，也在琢磨怎么把大模型真正塞进业务里。<br>
&emsp;&emsp;代码对我而言，不只是逻辑，更像是一种表达方式——用接口抽象混乱，用数据串联关系。<br>
&emsp;&emsp;最近越来越觉得，让一段后端代码因为 AI 的加入而变得稍微有点温度，是件挺浪漫的事。<br>
&emsp;&emsp;喜欢折腾，也喜欢把折腾的过程记录下来。生活里除了 0 和 1，还有构建完成后的会心一笑。

</td>
</tr>
</table>

---

### 🛠️ 近期折腾

- 用 Spring AI 把 RAG 塞进老系统，在检索效果和响应速度之间反复横跳
- 在 Neo4j 里画关系网，每次看到那些节点和连线，都觉得自己在画地图
- 刷 LeetCode，不是为别的，只是觉得把一道 hard 题捋顺的那一刻，整个世界都变清晰了

---

### 📦 几个自己觉得还不错的项目

| 项目 | 一句话 | 用到的技术 |
| :--- | :--- | :--- |
| AI 外卖助手 | 让外卖系统学会说“人话”——RAG 智能问答 + 订单自然语言查询 | Spring Boot / Spring AI / 向量数据库 |
| 图推荐系统 | 用图替代 JOIN，让“你可能认识的人”变得真的可能认识 | Neo4j / Spring Data / Redis |
| 社区论坛 | 校园里的技术后花园，楼中楼、全文检索、积分体系全都有 | Spring Boot / MySQL / Elasticsearch |
| I-Agent | 个人 AI 助手，SSE 流式对话，让它记住你说过的每一句话 | Spring AI 2.0 / DeepSeek / Qdrant |
| LeetCode 记录 | 刷题存档，顺便看看自己写代码的思路有没有进化 | Java |

---

### 📊 一些数字

<div align="center">

  <!-- 活动图 -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=34204002&theme=tokyo-night&hide_border=true&area=true" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=34204002&theme=github-light&hide_border=true&area=true" />
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=34204002&theme=tokyo-night&hide_border=true&area=true" width="98%" alt="activity graph" />
  </picture>

  <!-- 三栏统计 -->
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=34204002&theme=tokyonight&utcOffset=8" width="32%" alt="productive time" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=34204002&layout=compact&hide_border=true&theme=tokyonight&langs_count=6&include_all_forks=true&hide=html,css,javascript" width="32%" alt="top langs" />
  <img src="https://github-readme-streak-stats.herokuapp.com?user=34204002&theme=tokyonight&hide_border=true" width="32%" alt="streak stats" />

</div>

---

### 📬 联系我

- 邮箱：34204002@qq.com
- 聊技术、聊项目，或者只是单纯想喝杯咖啡，都欢迎。

---

<div align="center">
  <sub>Made with ☕, curiosity, and a bit of late-night debugging.</sub>
</div>

<!--
=========================================
📌 关于贪吃蛇贡献图
=========================================
想让贪吃蛇动起来，你需要在你的同名仓库 (34204002) 中配置一个 GitHub Action。
参考：https://github.com/Platane/snk

简单步骤：
1. 在仓库里创建 .github/workflows/snake.yml 文件
2. 复制下面的内容并提交
3. 等待 Actions 运行完毕，就可以看到效果了

示例 workflow：

name: generate snake
on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: Platane/snk@v3
        with:
          github_user_name: 34204002
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

配置完成后，上面那幅贪吃蛇图就会根据你的实际提交记录动起来了。
-->
