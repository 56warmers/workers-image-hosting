### MJJ最爱，基于cloudflare workers数据存储于KV的图床

------------

#### 方便实用，只需要更改wrangler.toml绑定的kv_id即可使用
#### 超级超级超级简单的Material 风(就一个按钮😂😂😂)
#### [DEMO](https://img.giao111.workers.dev/ "DEMO")

#### 使用:在 根目录和static目录输入

    npm i
	
#### 	再进入static目录编译Vue
    npm run build
#### 	之后修改wrangler.toml


    kv_namespaces = [
      { binding = "LINK", id = "11111",preview_id='11111'}//ID修改为自己创建的KV的id，preview_id是dev环境绑定的kv可以去掉
    ]
### 	之后在根目录执行


    wrangler publish
#### 	就OK了

------------

#### 可以访问 /list.html 路径查询已经上传的照片信息
#### 用户名+密码默认为123
#### 可以在/src/index.js中修改
