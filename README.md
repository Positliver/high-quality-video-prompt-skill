# High Quality Video Prompt Skill

一个可直接放进 GitHub、也可作为 OpenClaw / ClawHub Skill 发布的标准版中文 Skill 包。

它的作用是：把普通视频创意升级成更接近“导演分镜 + 摄影指导 + 美术设定 + 灯光设计 + 音效设计 + VFX 说明”的高质感提示词。

## 适用场景
- 人物出场片
- 品牌广告片
- 产品质感片
- 时尚影像
- 电影感短预告
- 科幻 / 奇幻 / 赛博朋克 / 悬疑风视频

## 仓库结构
```text
high-quality-video-prompt-skill/
├── SKILL.md
├── README.md
├── PUBLISHING.md
├── CHANGELOG.md
├── LICENSE
├── VERSION
├── templates/
├── examples/
└── assets/
```

## 本地安装到 OpenClaw
把整个文件夹放到以下任一位置：
- `<workspace>/skills/high-quality-video-prompt-skill`
- `~/.openclaw/skills/high-quality-video-prompt-skill`

然后开启新会话或重启 Gateway。

## 发布到 ClawHub
发布前先安装并登录 ClawHub CLI：
```bash
npm i -g clawhub
clawhub login
```

单独发布这个 skill：
```bash
clawhub publish ./high-quality-video-prompt-skill   --slug high-quality-video-prompt-skill   --name "High Quality Video Prompt Skill"   --version 1.0.0   --tags latest,video,prompt,cinematic
```

或者把本地 skills 一起扫描并同步：
```bash
clawhub sync --all
```

## 推荐使用顺序
1. 先看 `SKILL.md`
2. 用 `templates/quick-template.md` 或 `templates/prompt-fill-form.md` 起稿
3. 需要精修时切到 `templates/master-template.md`
4. 最后用 `assets/checklist.md` 自查

## 说明
- `SKILL.md` 已补齐 OpenClaw 所要求的 YAML frontmatter。
- `name` 使用 snake_case：`high_quality_video_prompt_skill`
- 目录名与建议 slug 使用 kebab-case：`high-quality-video-prompt-skill`
