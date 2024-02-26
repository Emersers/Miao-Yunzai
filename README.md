# Miao-Yunzai v3

基于乐神版[云崽v3.0](https://gitee.com/le-niao/Yunzai-Bot) 改造

需要同时安装[miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin.git) ，且后续的一些底层改造可能会改变数据结构，无法直接迁回原版Yunzai，请根据自己需求情况慎重安装

使用[icqq](https://github.com/icqqjs/icqq) 登录，防止oicq可能出现的低版本问题

项目仅供学习交流使用，严禁用于任何商业用途和非法行为

## 使用方法

> 环境准备： Windows or Linux，Node.js（ [版本至少v16以上](http://nodejs.cn/download/) ）， [Redis](https://redis.io/docs/getting-started/installation/ )

1.克隆项目并安装miao-plugin

请根据网络情况选择Github安装或Gitee安装

```
# 使用 Github 
git clone --depth=1 https://github.com/emersers/Miao-Yunzai.git
cd Miao-Yunzai 
git clone --depth=1 https://github.com/emersers/miao-plugin.git ./plugins/miao-plugin/


# 使用Gitee
git clone --depth=1 https://gitee.com/emersers/Miao-Yunzai.git
cd Miao-Yunzai 
git clone --depth=1 https://gitee.com/emersers/miao-plugin.git ./plugins/miao-plugin/
```

2.安装[pnpm](https://pnpm.io/zh/installation) ，已安装的可以跳过

```
# 使用npmjs.org安装
npm install pnpm -g

# 指定国内源npmmirror.com安装
npm --registry=https://registry.npmmirror.com install pnpm -g
```

3.安装依赖

```
# 直接安装
pnpm install -P

# 如依赖安装缓慢或失败，可尝试更换国内npm源后再执行install命令
pnpm config set registry https://registry.npmmirror.com
pnpm install -P
```

4.运行（首次运行按提示输入登录）

```
node app
```