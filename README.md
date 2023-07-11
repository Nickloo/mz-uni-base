# mz-uni-base

## app开发先npx @dcloudio/uvm

### Android打包配置

* 应用签名: 
### 配置
#### 主题色配置

- uni.scss 中引入
``` scss
// 引入样式
@import './common/styles/index.scss';

$mz-primary:#ffffff; // 覆盖原有颜色
$u-primary:#ffffff; // 覆盖uview的主题色

```
- 使用插件时设置配置

``` javascript
import mzCommon from './common'

Vue.use(mzCommon, {
  socket: {
    url: socketIO.url,
    token: store.state.user.token,
    onConnect() {
      console.log('onConnect')
    },
    onMessage(message) {
      console.log('onMessage', message)
    },
    
  },
  store,
  themeColor: '#FD2727'
})
```
