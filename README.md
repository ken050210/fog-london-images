# 雾都秘史 · 图床

角色卡《雾都秘史》使用的图片。卡片通过 manifest.json 找图；卡内只带小尺寸地图兜底，酒馆允许外部媒体时才从这里加载原图。

- `manifest.json`：图床索引，由卡片项目的 `node tools/make-image-index.mjs 图床` 生成。
- `maps/`：手记地图原图（london 伦敦、mansus 漫宿、world 醒时世界）。
- `portraits/`：20 位人物的立绘，用在手记的“此刻相逢”（原图尺寸 832×1216，WebP）。
- `avatars/`：对白框用的方形头像，从上半身证件照裁出（按裁剪框的原始像素，约 690–830 像素见方，WebP）。
- 立绘与头像用 NovelAI Diffusion V5 生成。

更新图片后重新生成 manifest.json 再提交。jsDelivr 会缓存一段时间（最长约 12 小时），急用可以打开 `https://purge.jsdelivr.net/gh/<用户名>/<仓库>@main/manifest.json` 刷新。

《雾都秘史》is unofficial content based on Cultist Simulator and BOOK OF HOURS by Weather Factory Ltd. 本仓库图片属于非官方同人作品，未经 Weather Factory 认可。
