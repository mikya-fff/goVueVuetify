# Go +  Vue +Vuetify

## Vue

https://cn.vuejs.org/

### ubuntu安装

https://cn.vuejs.org/v2/guide/installation.html

#### 依赖环境

- Node.js

  ubuntu默认已经安装，使用`node -v`来查看

- npm

  ` sudo apt-get install npm`来安装

- cnpm

  由于网络的问题，使用中国的npm，网速更快

  ```bash
   sudo npm install -g cnpm --registry=https://registry.npm.taobao.org
  ```

#### 安装

```bash
sudo cnpm install -g @vue/cli
```

## Vuerity

https://vuetifyjs.com/zh-Hans/

### 安装

1.先创建一个vue项目

```bash
vue create vuetify-demo

#根据提示选择相应的选项,输出如下

Vue CLI v4.5.13
? Please pick a preset: Manually select features
? Check the features needed for your project: Choose Vue version, Babel, Router, Vuex, CSS Pre-processors
? Choose a version of Vue.js that you want to start the project with 2.x
? Use history mode for router? (Requires proper server setup for index fallback in production) No
? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Sass/SCSS (with dart-sass)
? Where do you prefer placing config for Babel, ESLint, etc.? In dedicated config files
? Save this as a preset for future projects? Yes
? Save preset as: vueapp_config_demo

🎉  Preset vueapp_config_demo saved in /home/mikya/.vuerc


Vue CLI v4.5.13
✨  Creating project in /home/mikya/gitlab/goVueVuetify/vuetify-demo.
⚙️  Installing CLI plugins. This might take a while...


> core-js@3.12.1 postinstall /home/mikya/gitlab/goVueVuetify/vuetify-demo/node_modules/core-js
> node -e "try{require('./postinstall')}catch(e){}"


> ejs@2.7.4 postinstall /home/mikya/gitlab/goVueVuetify/vuetify-demo/node_modules/ejs
> node ./postinstall.js

added 1207 packages from 639 contributors in 20.277s

68 packages are looking for funding
  run `npm fund` for details

🚀  Invoking generators...
📦  Installing additional dependencies...

added 9 packages from 5 contributors in 4.382s

69 packages are looking for funding
  run `npm fund` for details

⚓  Running completion hooks...

📄  Generating README.md...

🎉  Successfully created project vuetify-demo.
👉  Get started with the following commands:

 $ cd vuetify-demo
 $ npm run serve

```

2.安装vuetify插件

```bash
vue add vuetify

#输出内容如下

? Still proceed? Yes

📦  Installing vue-cli-plugin-vuetify...

+ vue-cli-plugin-vuetify@2.4.0
added 9 packages from 11 contributors in 4.569s

69 packages are looking for funding
  run `npm fund` for details

✔  Successfully installed plugin: vue-cli-plugin-vuetify

? Choose a preset: Default (recommended)

🚀  Invoking generator for vue-cli-plugin-vuetify...
 WARN  conflicting versions for project dependency "sass-loader":

- ^8.0.2 injected by generator "undefined"
- ^10.0.0 injected by generator "vue-cli-plugin-vuetify"

Using newer version (^10.0.0), but this may cause build errors.
📦  Installing additional dependencies...

added 13 packages from 8 contributors, removed 2 packages and updated 1 package in 9.05s

72 packages are looking for funding
  run `npm fund` for details

⚓  Running completion hooks...

✔  Successfully invoked generator for plugin: vue-cli-plugin-vuetify
 vuetify  Discord community: https://community.vuetifyjs.com
 vuetify  Github: https://github.com/vuetifyjs/vuetify
 vuetify  Support Vuetify: https://github.com/sponsors/johnleider
```

3.启动一个vue应用

```bash
$ cd vuetify-demo
$ npm run serve

#输出如下

  App running at:
  - Local:   http://localhost:8080/ 

  Note that the development build is not optimized.
  To create a production build, run npm run build.

```

4.如果需要部署到服务器，需要编译一下,

```bash
npm run build
```

生成的文件在`dist`目录下,直接把这个目录放到服务器上的即可。
