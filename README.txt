AI抢饭碗_真人版 — 免费托管资产说明
=====================================
本文件夹内含 OmniHuman 需要的全部输入：
  - aqiang.jpg      角色「阿强」真人肖像
  - linzong.jpg     角色「林总」真人肖像
  - seg_01_aqiang.mp3 ... seg_14_linzong.mp3  14 段对口型音频

只需把整个 host_assets/ 传到任意【免费、公网可访问】的静态托管，
然后把文件的公开 URL 给我即可。推荐方式：GitHub 公开仓库 + jsDelivr CDN。

--- 方式 A：GitHub + jsDelivr（推荐，免费、稳定、持久）---
1. 登录 GitHub，新建一个【Public】仓库（如 ai-drama-assets）。
2. 把 host_assets/ 里所有文件拖进仓库（或用 git push）。
3. 假设用户名 user、仓库 ai-drama-assets、分支 main，则：
   图片 URL: https://cdn.jsdelivr.net/gh/user/ai-drama-assets@main/aqiang.jpg
   音频 URL: https://cdn.jsdelivr.net/gh/user/ai-drama-assets@main/seg_01_aqiang.mp3
   （把 user / 仓库名 / 分支替成你的实际值，文件名保持本文件夹原名）
4. 把「user/ai-drama-assets@main」这样的信息发我，我直接拼出 16 个 URL。

--- 方式 B：GitHub Pages / Cloudflare Pages / Netlify / Vercel ---
   任意免费静态托管，上传后给每个文件的公开 URL 即可。

--- 方式 C：临时公网（不推荐，易失效）---
   本地起 HTTP 服务 + cloudflared/ngrok 临时隧道，生成临时 URL；
   需在整个生成期间保持隧道在线，较脆弱。

注意：OmniHuman 服务端会主动拉取这些 URL，所以必须是「无需鉴权、公网可达」的地址。
