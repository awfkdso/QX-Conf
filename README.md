# QX-Conf
本人自用的QX配置，给有需要的朋友分享，本配置中大量引用了各位大佬的代码，表示感谢！！

[task_local]
本地任务，按照配置文件注释中的JSON地址去追加，每追加一个的类似多一个商店。
在商店中再按需添加自己所需的功能。具体哪个有什么功能，只能自己摸索了。

[policy]
策略组，主要分为 手动主，地区最优（自动），各种媒体，地区手动 和 终极清单
手动主：就是主节点，第一梯队的候选就是地区最优（自动），保证落到最快的可用节点上
地区最优：就是每个地区中响应最快的节点，每10分钟检测一次响应速度并自动调整节点。
各种媒体：自己按需选择对应地区的节点
地区手动：建议自己手动选好哪个可以解锁流媒体
终极清单：选择代理或不代理，决定了整个策略是白名单还是黑名单。

[server_remote]
远程服务器，此处自行添加机场订阅或节点

[filter_remote]
远程分流，目前对我个人而言是大而全的配置，可以自行删减，并按照注释中的去追加。
广告规则由于有大量重复，所有不能全部同时开启，现在默认配置就很好。

[rewrite_remote]
远程重写，参考大量大佬的重写规则，可自行调整打开或关闭

[mitm]
中间人伪装，主要用于处理HTTPS流量数据。
很多远程重写的规则，依赖于hostname定义的域名才能够真正生效。
因此目前此处可能有很多不足，将来有时间再补充。