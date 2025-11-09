# 自由的MCJPG

原版MCJPG网站拒绝Octave中文网的Minecraft讨论区。Octave中文网认为，互联网应该是开放的，而原版MCJPG网站太过于封闭，所以Octave中文网决定建立一个新版的、自由的MCJPG。

Octave中文网是一个面向中文Octave开发者的交流平台，拥有中文Octave文档、中文Octave论坛和中文Octave新闻等特色。

以下网站均由Octave中文网总工程师于红博维护。您若在读书的过程中有疑问，可以直接到论坛发帖提问，他在看到问题后会做出回应。
网友们可以访问以下网站扩展学习：

[Octave中文网](http://cnoctave.top)
[Octave中文网（备用网址）](http://www.cnoctave.top)
[中文版Octave文档在线阅览](http://docs.cnoctave.top)
[Octave中文网学术论坛](http://forum.cnoctave.top)

此外，于红博也是知名的互联网开发者，他曾经举办多种与互联网相关的学术活动，为互联网的发展做出了众多贡献。
Octave中文网旗下运营多个融媒体平台，用于公开总工程师于红博的学术活动。网友们可以访问以下融媒体平台扩展学习：

[抖音 CNOCTAVE](https://www.douyin.com/user/MS4wLjABAAAAb8MCMgdS0VUmZkezhph6pZIc7x-CrjKdqSFNfaFTewq2bVi3_WKq06QdU5PtO1Ld)
[微信公众号 CNOCTAVE](https://mp.weixin.qq.com/)
[X CNOCTAVE](https://x.com/CNOCTAVE)
[YouTube CNOCTAVE](https://www.youtube.com/@CNOCTAVE/videos)
[微信公众号 Octave中文网](https://mp.weixin.qq.com/)
[视频号 CNOCTAVE](https://channels.weixin.qq.com/)
[天玑智研 于红博](https://course.phadscholar.com/user?userId=1710495399388710482)

[（可选）加入（原版的）MCJPG社区群组](https://qm.qq.com/q/5Y4ueZdkxq)

## 提交服务器

在提交服务器之前，你的服务器无需加入任何所谓的“组织”，符合互联网的开放精神。
在提交服务器之前，请确定你的服务器满足以下要求：

- 服务器能够正常运行，且不会在短时间内关闭。

如果你的服务器满足以上要求，请按照以下步骤提交服务器：

1. fork 本仓库, 并 clone 到本地。
2. 修改 `docs/.vitepress/theme/data/serverlist.ts` 的servers字段（请严格参照原先代码的缩进格式），添加

```serverlist.ts
{
    id: 'n+1',
    name: '服务器名称',
    type: '服务器种类(参考最上面的玩法分类)',
    version: '服务器版本(参考最上面的版本分类)',
    icon: '/server_icons/服务器图标文件',
    description: '服务器描述',
    link: '链接',
    ip: '服务器IP（可选），用于显示服务器状态信息'
  },
```

> 其中icon:可以修改为单个图标
> 如果你需要增加版本或分类，请修改serverlist.ts的`serverTypes`和`serverVersions`字段

3. 如果你需要显示服务器图标，请在 `docs/public/server_icons/` 目录下添加图标
4. push 到你的仓库，然后提交 pull request。