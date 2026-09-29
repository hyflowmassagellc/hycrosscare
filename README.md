# HyCross Health — 官网静态文件

三个语言版本,跟Bonavia那套部署方式完全一样(你已经熟悉整个流程了):

- `index.html` — 英文版(首页)
- `ru.html` — 俄文版
- `fr.html` — 法文版
- `CNAME` — 内容是 `hycrosscare.com`,和其他文件一起上传即可,不用改
- `sitemap.xml` / `robots.txt` — 直接一起传到仓库根目录

## 部署步骤(和Bonavia一模一样)

1. GitHub 新建一个 Public 仓库(比如叫 `hycrosscare`)
2. 把这六个文件全部拖进仓库根目录,Commit
3. Settings → Pages → Source选`Deploy from a branch` → Branch选`main`,目录`/ (root)` → Save
4. Custom domain 填 `hycrosscare.com`,Save
5. 去 Namecheap 该域名的 Advanced DNS,加同样的5条记录(4条A记录 + 1条CNAME),**记得删掉Namecheap默认自带的parking page CNAME记录和URL Redirect记录**,不然会冲突
6. 等DNS生效,回GitHub点Check again,生效后勾选Enforce HTTPS

## 还需要你确认/补充的真实信息

- **邮箱**:目前用的是 `info@hycrosscare.com` 作为默认建议,如果你想用别的邮箱,告诉我改
- **电话**:还是占位符 `[+1 (000) 000-0000]`,需要真实号码
- **响应时间**:表单说明里的"[响应时间]"还没填,之前Bonavia用的是24小时,HyCross要不要用同一个,或者不同的承诺时间(比如更快或更慢),告诉我
- **表单后端**:同样需要注册一个Formspree账号(用你想接收HyCross咨询的邮箱),拿到表单ID发给我,我帮你接进三个页面
