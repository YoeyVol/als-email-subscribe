# ALS 邮件订阅中心 / ALS Email Subscription Hub

一页式静态网站，汇总渐冻症（ALS / MND）官方组织的 **邮件 / newsletter 订阅入口**。  
点击「订阅邮件」会在新标签页打开对应组织的官方订阅页；**本站不收集、不存储任何邮箱**。

A one-page static hub that links to official ALS/MND organization newsletter signup pages.  
This site does **not** collect email addresses; buttons open the organizations’ own forms.

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

## GitHub Pages

仓库根目录即为站点根目录（`index.html`）。在仓库 Settings → Pages 中选择分支 `main`、文件夹 `/ (root)` 即可发布。

Expected URL pattern: `https://<username>.github.io/als-email-subscribe/`

## 商标 / Trademarks

各组织名称与 Logo 均为其各自所有者的商标或标识，仅用于识别对应官方订阅入口，不代表本站与这些组织存在隶属或背书关系。

## 未收录 / Not included

- **Answer ALS**：公开网站上未找到明确的 newsletter 订阅表单（仅有历史通讯稿与联系邮箱），故暂未收录。

## License

站点代码（HTML/CSS）可自由使用。Logo 文件仍归原组织所有，请勿另行商用再分发。
