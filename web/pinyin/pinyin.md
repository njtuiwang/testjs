/*
Title: pinyin
Description: pinyin
*/

# 功能描述
pinyin是汉字转拼音工具，支持20870个汉字，包含完整的多音字，压缩57kb

# 依赖模块
无

# 快速使用

```js
parsePinyin('阿里巴巴', function (charactor, spell) {
    if (charactor === '阿') {
        return spell[1]
    }
    return spell[0];
})
```

## 配置项

### 参数1
* 类型：String
* 作用：汉字字符串
* 是否必传：是
### 参数2
* 类型：Function
* 默认值：无
* 作用：多音字处理函数，默认全部返回
* 是否必传：否
