通常我们会为同一个源站创建多条加速通道，以覆盖多个加速区域的用户。如果需要实现多个区域的用户接入同一个域名访问源站，您可以通过配置 DNS 的方式来达到统一域名、就近接入的目的。

如果您开通了通道组的服务。可以开通通道组的全球统一域名接入的服务，您将获得一个统一的域名，同时还可以通过配置界面精准调整通道覆盖的加速区域，让用户通过通道或者公网访问源站区域。

## 开通统一域名接入

在通道组列表里，单击通道组 ID 或名称，打开通道组详情页，选择顶部的“全球统一域名接入”标签：

![](https://main.qcloudimg.com/raw/153e67534e7a49bce047209f07486ef8.png)

仔细阅读相关的说明后，单击【开通服务】。

![](https://main.qcloudimg.com/raw/2c114cd64be71a6ee2ccd281ee8b599d.png)

服务开通后，系统将通过通道组所包含的加速通道，配置了每一条加速通道所覆盖的加速区域，加速区域的默认原则是距离入口近，或者公网访问入口延时较低的区域。

## 配置加速区域

当您开通了统一域名接入服务后，系统将为您的每一条通道配置了默认的加速区域，如果您觉得这些加速区域不够精准，可以单击左边的【修改】链接，对加速区域进行调整，增加或者减少覆盖区域，以达到精准覆盖的目的。

![](https://main.qcloudimg.com/raw/2fed708fb9f360ba9b63983b8444b6e9.png)

调整完毕后，单击【确认】按钮更新并保存。

## 配置默认入口

启用全球统一域名接入后，全球的用户将通过该域名访问源站，您需要处理以下几种用户的访问路径，否则会出现因绕路而导致不必要的网络延时，以及产生不必要的流量费用：

- **源站区域用户**：原则上源站区域的用户只需要通过公网直连即可以获得最低的延时，不需要使用加速通道访问源站。
- **离源站区域距离较近，或远离加速通道入口的区域**：这些区域用户通过公网直连就能得到不错的低延时，接入加速通道并不能保证效果更好。

在配置加速区域的页面，我们提供了一个 “默认入口” ，当您配置了该入口的 IP 地址后，意味着除了加速通道所覆盖的区域用户外，其他区域的用户将通过公网直连该 IP 地址，从而访问您的源站。

单击 “默认入口” 右侧的【修改】链接，弹出输入 IP 地址的对话框：

![](https://main.qcloudimg.com/raw/79702e1970c9fa9b763f9da93356f213.png)

输入 IP 地址后，单击【确认】。**返回详情页，单击【保存】按钮，以便修改能得到更新。**

![](https://main.qcloudimg.com/raw/8af4dd0cd137597641a2b40a245af25f.png)

