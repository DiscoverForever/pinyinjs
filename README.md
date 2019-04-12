# pinyinjs
中文转拼音工具
本项目基于pinyinjs项目修改
项目地址https://github.com/sxei/pinyinjs
# 安装
```bash
npm i pinyinjs --save
```
# 如何使用

封装好的3个方法：

```javascript
const pinyinUtil = require('pinyinjs')
/**
 * 获取汉字的拼音首字母
 * @param str 汉字字符串，如果遇到非汉字则原样返回
 * @param polyphone 是否支持多音字，默认false，如果为true，会返回所有可能的组合数组
 */
pinyinUtil.getFirstLetter(str, polyphone);
/**
 * 根据汉字获取拼音，如果不是汉字直接返回原字符
 * @param str 要转换的汉字
 * @param splitter 分隔字符，默认用空格分隔
 * @param withtone 返回结果是否包含声调，默认是
 * @param polyphone 是否支持多音字，默认否
*/
pinyinUtil.getPinyin(str, splitter, withtone, polyphone);
/**
 * 拼音转汉字，只支持单个汉字，返回所有匹配的汉字组合
 * @param pinyin 单个汉字的拼音，不能包含声调
 */
pinyinUtil.getHanzi(pinyin)；
```
