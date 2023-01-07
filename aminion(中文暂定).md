## UI
- 移动端
- web

### 网页功能
> 插件只是展示缩略的信息，它是正式版的内容，有着完整的体验内容。继续使用vue搭建

```shell
npm create vite@latest my-vue-app --template vue
npm install vue-router@4

```
- 登录退出
	- [ ] 超过7天自动退出
	- [ ] 密码修改，全局退出
	- [ ] 登录设备管理
- 收藏内容
	- [ ] 不支持修改收藏内容，支持增加批注，注释功能
	- [ ] 删除功能
	- [ ] 置顶
	- [ ] 公开 / 私有
	- [ ] 支持导出(txt, md格式)
- 笔记功能
	- [ ] 公开 / 私有
	- [ ] 删除
	- [ ] 置顶
	- [ ] 修改
	- [ ] 富文本编辑(支持markdown)
	- [ ] 支持导出
- Todo List
- 个人信息自己管理
- 回收站功能（7天内的内容可以恢复）

#### 设计



### 插件功能
- 登录/退出(设定7天退出)
- 收藏选中的内容
- 收藏内容展示和删除
- 笔记功能
- 收藏夹功能（优化系统的收藏）
- 单词展示 / 单词查询存储

### 第一步
- 构建页面（Vue）

## 功能细节描述

**登录**
插件端不可注册
移动端可注册
登录流程


## 创建工程


```shell
npm create vite@latest # 安装vite

npm i @crxjs/vite-plugin@beta -D # 安装vite

npm install @icon-park/vue-next --save # 安装iconpark 库

npm install --save qrcode.vue # 安装vue生成二维码工具

npm install pinia # pinia 工具

npm install @tiptap/vue-3 @tiptap/starter-kit # 富文本编辑器
	npm install @tiptap/extension-typography # 插件
	

```

- 目前`manifest`配置
```json
{

  "manifest_version": 3, // 必须

  "name": "aminion", // 必须

  "description": "a chrome plugin",

  "version": "0.1.0", // 必须

  "action": { "default_popup": "index.html" },

  "author": "leeweo",

  "content_scripts": [

    {

      "js": ["src/content.ts"],

      "matches": ["<all_urls>"]

    }

  ],

  "background": {

    "service_worker": "src/background.ts",

    "type": "module"

  }

}
```

