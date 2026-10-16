# ALS 邮件订阅中心 / ALS Email Subscription Hub

一页式静态网站，汇总渐冻症（ALS / MND）官方组织的 **邮件 / newsletter 订阅入口**。  
点击「订阅邮件」会在新标签页打开对应组织的官方订阅页；**本站不收集、不存储任何邮箱**。

A one-page static hub that links to official ALS/MND organization newsletter signup pages.  
This site does **not** collect email addresses; buttons open the organizations’ own forms.

## 已收录组织 / Included organizations

| 组织 | 订阅页 | Logo 来源 |
|---|---|---|
| The ALS Association | https://www.als.org/newsletter-sign-up | Wikimedia / als.org brand |
| ALS News Today | https://alsnewstoday.com/newsletter/ | alsnewstoday.com 官方 SVG |
| ALS TDI | https://www.als.net/subscribe/ | als.net 官方 SVG |
| I AM ALS | https://www.iamals.org/news/newsletter/ | iamals.org 官方 PNG |
| Project ALS | https://projectals.org/subscribe-to-our-newsletter/ | projectals.org 官方 PNG |
| ALS Canada | https://als.ca/#gf_1 （首页订阅表单） | als.ca 官方 PNG |
| Target ALS | https://targetals.org/join-us/ | targetals.org 官方 SVG |
| Healey & AMG Center for ALS | https://lp.constantcontactpages.com/sl/wQfOqgA/ALSLink | Mass General 官方 SVG |
| FightMND (AU) | https://fightmnd.org.au/ （页脚 newsletter） | fightmnd.org.au 官方 SVG |
| MND Association (UK) | https://www.mndassociation.org/research/for-researchers/noticeboard/the-researcher-newsletter | Wikimedia Commons |

## 未收录 / Not included

- **Answer ALS**：公开网站上未找到明确的 newsletter 订阅表单（仅有历史通讯与联系邮箱），故暂未收录。

## 使用 / How to use

1. 打开站点首页。
2. 在卡片上点击 **订阅邮件**。
3. 在对方官网完成订阅（姓名、邮箱、兴趣选项等由对方处理）。

## 本地预览 / Local preview

```bash
cd als-email-subscribe
python3 -m http.server 8080
# open http://localhost:8080
```

## 发布到 GitHub Pages

```bash
gh auth login
gh repo create als-email-subscribe --public --source=. --remote=origin --push
gh api -X POST repos/YoeyVol/als-email-subscribe/pages \
  -f build_type=legacy \
  -f source='{"branch":"main","path":"/"}'
# 预计地址：https://yoeyvol.github.io/als-email-subscribe/
```

## 商标 / Trademarks

各组织名称与 Logo 均为其各自所有者的商标或标识，仅用于识别对应官方订阅入口，不代表本站与这些组织存在隶属或背书关系。

## License

站点代码（HTML/CSS）可自由使用。Logo 文件仍归原组织所有，请勿另行商用再分发。
