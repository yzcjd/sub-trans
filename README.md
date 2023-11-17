## Cloudflare Workers 实现订阅转换

### 需要物品：
1. 别人的订阅转换站（如[肥羊](https://api.v1.mk)）
2. Cloudflare

#### 1. Cloudflare 创建 Workers
① 进入 Cloudflare 控制面板，点击左侧导航栏 Workers & Pages，然后点击 Create Worker

![](https://github.com/yzcjd/sub-trans/blob/main/png/1.png?raw=true)

② 输入 Worker 的名字，点击 Deploy



③ 点击 Edit Code，进入代码编辑器



④ 在左侧编辑器输入代码后，点击右上角的 Save and deploy 即可




⑤ 部署 Worker

⑥ 复制 sub-trans.worker.js 文件内容到 worker.js 中

⑦ 变量中添加 BACKEND，值为后端地址例如 https://api.v1.mk 或 https://sub.id9.cc



⑧ 创建一个 KV，命名空间名可以随意填写



⑨ 返回 Worker 的设置中，找到下方的 KV Namespace Bingdings，变量名为 SUB_BUCKET



##### 1.订阅转换
① 如访问 https://xxx.workers.dev ，不用修改；
② 如访问别人的订阅转换，如 [Subscription Converter](https://sub-web.netlify.app/) 将后端地址修改为自己搭建的地址。




### 可以直接用我的： sub-converter.yzcjd.workers.dev

### 参考资料
##### 参考不良林教程 https://www.youtube.com/watch?v=X7CC5jrgazo
##### 参考Github项目 https://github.com/bulianglin/psub

（以后加图片）
