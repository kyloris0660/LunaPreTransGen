# LunaPreTransGen

## 还在写

LunaPreTransGen 是一个用于生成 LunaTranslator 预翻译文件的工具。

它从解包的文本文件中读取内容，通过API将这些文本翻译为中文，生成适用于 LunaTranslator 的预翻译文件。用于节省每次hook出文本后翻译的时间并在一定程度上（？）强化上下文联系。适合有一定日语基础和解包基础并习惯使用LunaTranslator 进行辅助的极少数用户。如不符合上述需求，建议直接使用[GalTrans](https://github.com/xd2333/GalTransl) 。目前支持openai兼容接口的多种翻译。

## 兼容json格式

如，常见于[VNTextPatch](https://github.com/arcusmaximus/VNTranslationTools)：

```json
[
  {
    "name": "XXX",
    "message": "「XXX」"
  },
  {
    "message": "XXX。"
  }
]
```

实现参考了 [GalTrans](https://github.com/xd2333/GalTransl) 的设计思想与功能。

