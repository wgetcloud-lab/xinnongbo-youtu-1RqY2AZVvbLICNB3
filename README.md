[合集 \- 经验分享(27\)](https://github.com)[1\.记一次由于操作失误致使数据库瘫痪的故障分析与解决方案2023\-09\-08](https://github.com/guoxiaoyu/p/17678340.html)[2\.网络之谜：记一次失败排查的故事2023\-11\-15](https://github.com/guoxiaoyu/p/17811098.html)[3\.你是否想知道如何应对高并发？Go语言为你提供了答案！2023\-12\-29](https://github.com/guoxiaoyu/p/17933653.html)[4\.2023年终总结：拉帮结伙，拼搏探索新机遇2023\-12\-30](https://github.com/guoxiaoyu/p/17933731.html)[5\.谁说后端不能画出美丽的动图？让我来给大家拜个年！01\-29](https://github.com/guoxiaoyu/p/17991503)[6\.【10秒开服】幻兽帕鲁全自动部署教程，难道你还想手动搭建游戏服务器吗？快来学习这个简单又快速的方法！01\-30](https://github.com/guoxiaoyu/p/17998193)[7\.踩坑指南：入门OpenTenBase之部署篇04\-10](https://github.com/guoxiaoyu/p/18116318)[8\.踩坑指南：入门OpenTenBase之监控篇04\-11](https://github.com/guoxiaoyu/p/18117472)[9\.加速博客体验：静态资源优化技巧大揭秘！04\-28](https://github.com/guoxiaoyu/p/18149525)[10\.5分钟带你了解RabbitMQ的（普通/镜像）集群06\-14](https://github.com/guoxiaoyu/p/18240661)[11\.金仓数据库全攻略：简化部署，优化管理的全流程指南06\-21](https://github.com/guoxiaoyu/p/18257320)[12\.KES数据库实践指南：探索KES数据库的事务隔离级别07\-02](https://github.com/guoxiaoyu/p/18276998)[13\.云端IDE如何重定义开发体验07\-24](https://github.com/guoxiaoyu/p/18294897)[14\.国产数据库：数字时代的科技巨擘07\-16](https://github.com/guoxiaoyu/p/18295131)[15\.浅析前端数据埋点监控：用户行为与性能分析的桥梁08\-02](https://github.com/guoxiaoyu/p/18329944):[蓝猫机场](https://fenfang.org)[16\.数据库与我：一段关于学习与成长的深情回顾08\-05](https://github.com/guoxiaoyu/p/18338820)[17\.观存储历史，论数据未来08\-12](https://github.com/guoxiaoyu/p/18352499)[18\.从自建到云原生：数据管理的未来与变革08\-13](https://github.com/guoxiaoyu/p/18354003)[19\.深入分析与解决方案：缓存与数据库双写不一致问题08\-20](https://github.com/guoxiaoyu/p/18363049)[20\.小白系列：数据库基础知识解析08\-19](https://github.com/guoxiaoyu/p/18363713)[21\.智能客服的演变：从传统到向量数据库的新时代08\-21](https://github.com/guoxiaoyu/p/18370513)[22\.Cloud Studio：颠覆传统的云端开发与学习解决方案08\-28](https://github.com/guoxiaoyu/p/18382973)[23\.单元测试的入门实践与应用09\-05](https://github.com/guoxiaoyu/p/18395944)[24\.Git冲突解决技巧09\-15](https://github.com/guoxiaoyu/p/18409072)[25\.提升软件测试效率与灵活性：探索Mock测试的重要性09\-22](https://github.com/guoxiaoyu/p/18419378)[26\.从设计到代码：探索高效的前端开发工具与实践09\-28](https://github.com/guoxiaoyu/p/18425801)27\.掌握Docker：简化KES单机安装与管理的最佳实践10\-01收起
今天我们将继续深入探讨KES的单机安装，依然围绕Docker的使用展开。这一部分的内容将涵盖一些常见的陷阱以及在遇到问题时如何进行有效的反馈和解决。首先，我们需要找到官方的安装教程，确保以官方指南为主，同时结合我们自己的使用习惯。


为什么我们如此青睐Docker，而不是选择传统的命令行安装呢？在当今的云计算时代，Docker已经成为一种几乎必备的技能，它能够大大简化环境配置和应用部署的流程，使得开发和运维工作更加高效。


接下来，我们将详细讲解具体的安装步骤和注意事项，帮助大家顺利完成KES的安装。让我们开始吧！


# 单机安装


在这里，我想与大家分享官方的安装步骤，您可以通过以下链接访问详细的安装指南：[官方安装步骤](https://github.com)。同时，如果您需要下载相关的软件或资源，请前往官方的下载地址：[官方下载页面](https://github.com)。


这些链接提供了全面的文档和工具，帮助您更顺利地进行安装和配置。建议大家在安装之前先仔细阅读官方指南，以便更好地理解每个步骤的具体操作和注意事项。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224529283-1417013114.png)


我已经为大家准备好了相关的下载链接，您可以通过以下地址获取所需文件：[下载地址](https://github.com)。


需要特别提醒的是，虽然这个链接中包含了中文字符，这并不会对下载过程产生实质性的影响，但从规范性和可读性角度来看，这样的链接格式并不太理想。因此，建议官方在未来的链接命名中尽量避免使用中文，以提高链接的清晰度和一致性。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224534380-1519384272.png)


我们将继续使用宝塔面板进行直接安装，因为我选择了 Docker 版本，这样我们可以直接导入镜像进行使用。需要注意的是，官方尚未对外公开可用于公网的官方镜像，因此这种方式是当前最方便的选择。


## 导入镜像


最初，我打算通过宝塔面板的导入镜像功能直接进行导入，但不幸的是，这一方法未能成功。因此，我只能转而使用命令行的方式进行导入。具体的命令如下：`docker load -i kingbase.tar`


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224541048-166920641.png)


此时，经过命令行的操作，本地环境中将成功生成所需的镜像，方便后续的使用和部署。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224546740-783663130.png)


我们决定直接采用 Compose 模板来启动服务，而不是使用官方提供的命令行形式。这种方式不仅能够简化配置过程，还能提高我们在多容器应用管理上的灵活性和效率。



```
version: "2"
services:
  kingbase:
    image: kingbase_v009r001c001b0030_single_x86:v1
    container_name: kingbase
    privileged: true  # 注意这里的缩进与前面的键值对对齐
    environment:
      - ENABLE_CI=yes    # yes(默认 大小写不敏感)/no 大小写敏感
      - NEED_START=yes    # yes(默认 启动数据库)/ no（不启动数据库）
      - DB_USER=system # 默认用户名
      - DB_PASSWORD=12345678ab  # 默认密码
      - DB_MODE=oracle    # 支持oracle/pg/mysql
    volumes:
      - /mnt/kingbase/data:/home/kingbase/userdata
    ports:
      - 4321:54321
    restart: unless-stopped
    command: /usr/sbin/init

```

编排模式的创建过程已经圆满完成，所有相关配置和设置已成功应用。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224553137-872780326.png)


接下来，我们将启动相应的模板，以便迅速搭建所需的环境和服务。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224559168-410104326.png)


## 启动服务


接下来，我们只需启动系统即可，相关的日志信息也非常清晰明了，有助于我们进行故障排查和性能监控。然而，我在这里遇到了一些问题，启动过程未能成功完成。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224639116-1128208198.png)


需要特别注意的是，由于我之前已经安装过一次 Kingbase，但在这次安装时忘记清空先前挂载的持久化目录，这导致了启动失败的情况。对于新手用户而言，通常在进行初次安装时，系统能够顺利启动并成功运行。


在成功安装的过程中，相关的日志信息清晰地显示了各项步骤和状态，以下是安装成功时的日志输出：


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224632951-209603801.png)


在成功启动后，我们可以直接进入容器内部进行免密码连接，以测试数据库的正常运行情况。首先，我们需要确认数据库服务是否已顺利启动：



> sys\_ctl \-D /home/kingbase/userdata/data/ status


其次，我们将进行免密码登录操作，以确保能够无缝地访问数据库：



> kql


我根据官方文档的指导进行操作，但直接显示为失败。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224625999-1508051244.png)


### 问题反馈


不过在安装过程中，您不必感到担忧，因为金仓官方提供了相应的问题论坛。在遇到任何困难时，您可以直接在论坛上发帖求助，寻求专业的支持与解答，论坛地址为：[https://bbs.kingbase.com.cn/forum。](https://github.com)


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224646462-2138449067.png)


那么我们暂时不使用免密登录的方式，而是直接使用刚才设定的默认账户和密码进行登录。



> ksql \-Usystem \-d test \-p54321


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224653249-629498683.png)


既然不存在相关数据库，我们可以直接登录后创建一个名为“system”的数据库，随后使用`ksql`命令进行免密登录。这种方法不仅简便，还能提高我们的工作效率。


至于我不太喜欢使用命令行的原因，是因为命令行操作需要配置多种环境信息，增加了出错的可能性。此外，命令行方式在未来的集群管理中可能会带来不便。目前，所有运维同事都倾向于使用Kubernetes来进行管理，因此Docker成为了主流的安装方式。这不仅简化了部署流程，还能更好地适应现代化的运维需求。


# 镜像推送


可以看出，官方并没有将镜像上传到Docker官方库，这意味着我们每次都需要到官网下载镜像。这种方式在操作时非常不便，尤其是在不同机器之间频繁切换时。因此，我们决定维护一个自己的镜像仓库，以便更高效地管理和部署。


这不仅可以大大简化我们的操作流程，还能确保在需要时能够快速获取所需镜像。目前，我以腾讯云为主要平台，而且个人实例的使用是免费的。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224708468-826283833.png)


创建一下镜像仓库：


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224712679-205100693.png)


我们在自己本地宝塔面板配置好仓库地址：


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224717263-297205153.png)


将我们已经导入好的镜像推送到自己的仓库是一个相对简单但至关重要的步骤。通过这一过程，我们可以确保这些镜像能够在需要时快速访问，从而大大提高工作效率。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224722867-187026170.png)


## 公有仓库


我已经成功地将镜像推送到了自己的公有仓库。这意味着在未来的操作中，如果你不愿意直接从官网下载镜像，也可以选择将所需的镜像直接下载。



```
version: "2"
services:
  kingbase:
    image: ccr.ccs.tencentyun.com/kingbase/database:v030
    container_name: kingbase-v030
    privileged: true  # 注意这里的缩进与前面的键值对对齐
    environment:
      - ENABLE_CI=yes    # yes(默认 大小写不敏感)/no 大小写敏感
      - NEED_START=yes    # yes(默认 启动数据库)/ no（不启动数据库）
      - DB_USER=system # 默认用户名
      - DB_PASSWORD=12345678ab  # 默认密码
      - DB_MODE=oracle    # 支持oracle/pg/mysql
    volumes:
      - /mnt/kingbase/data:/home/kingbase/userdata
    ports:
      - 4322:54321
    restart: unless-stopped
    command: /usr/sbin/init

```

由于我们已经拥有一个正在运行的数据库实例，这导致当前的新服务无法正常启动。


![image](https://img2024.cnblogs.com/blog/1423484/202409/1423484-20240927224730259-1101512075.png)


# 总结


在这个过程中，我们深刻感受到Docker作为现代开发与运维工具的重要性。从单机安装到镜像管理，每一步都体现出其高效性和灵活性。面对技术的快速迭代，保持对新工具的敏感和适应能力显得尤为关键。Docker不仅简化了环境配置，更为团队协作和资源共享提供了便利。


在实际操作中，虽会遇到各种问题，如镜像导入失败或启动过程中的小插曲，但这些都是成长过程中的必经之路。通过有效的问题反馈和社区支持，我们可以迅速找到解决方案，避免重复的错误。




---


我是努力的小雨，一名 Java 服务端码农，潜心研究着 AI 技术的奥秘。我热爱技术交流与分享，对开源社区充满热情。同时也是一位腾讯云创作之星、阿里云专家博主、华为云云享专家、掘金优秀作者。


💡 我将不吝分享我在技术道路上的个人探索与经验，希望能为你的学习与成长带来一些启发与帮助。


🌟 欢迎关注努力的小雨！🌟


