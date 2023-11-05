Cloudflare Workers 实现订阅转换
创建 Workers
进入 Cloudflare 控制面板，点击左侧导航栏 Workers & Pages，然后点击 Create Worker


输入 Worker 的名字，点击 Deploy


点击 Edit Code，进入代码编辑器


在左侧编辑器输入代码后，点击右上角的 Save and deploy 即可


部署 Worker
复制源代码到 worker.js 中
变量中添加 BACKEND，值为后端地址例如 https://api.v1.mk 或 https://sub.id9.cc


创建一个 KV，命名空间名可以随意填写


返回 Worker 的设置中，找到下方的 KV Namespace Bingdings，变量名为 SUB_BUCKET


订阅转换
访问 https://sub.username.workers.dev 或 Subscription Converter
将后端地址修改为自己搭建的地址（访问上面第一个地址的无需修改）

### 可以直接用我的： sub-converter.yzcjd.workers.dev

### 参考资料
##### 参考不良林教程 https://www.youtube.com/watch?v=X7CC5jrgazo
##### 参考Github项目 https://github.com/bulianglin/psub
##### 参考博客 https://zhichao.org/posts/ec29ee.html
