<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/juanfont/headscale/blob/main/docs/logo/headscale3_header_stacked_left.png"><img src="/juanfont/headscale/raw/main/docs/logo/headscale3_header_stacked_left.png" alt="头鳞标志" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/juanfont/headscale/actions/workflows/test.yml/badge.svg"><img src="https://github.com/juanfont/headscale/actions/workflows/test.yml/badge.svg" alt="词" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Tailscale 控制服务器的开源、自托管实现。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">加入我们的</font></font><a href="https://discord.gg/c84AZQhmpx" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Discord</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">服务器进行聊天。</font></font></p>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意：</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">始终选择与您使用的发布版本相同的 GitHub 标签，以确保您拥有正确的示例配置和文档。</font><font style="vertical-align: inherit;">该</font></font><code>main</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">分支可能包含未发布的更改。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">什么是尾鳞</font></font></h2><a id="user-content-what-is-tailscale" class="anchor" aria-label="永久链接：什么是尾鳞" href="#what-is-tailscale"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Tailscale 是一款构建在</font><a href="https://www.wireguard.com/" rel="nofollow"><font style="vertical-align: inherit;">Wireguard</font></a><font style="vertical-align: inherit;">之上的
</font></font><a href="https://tailscale.com/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">现代 VPN</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">它的工作方式类似于</font><font style="vertical-align: inherit;">
网络计算机之间的
</font><a href="https://tailscale.com/blog/how-tailscale-works/" rel="nofollow"><font style="vertical-align: inherit;">覆盖网络- 使用</font></a><a href="https://tailscale.com/blog/how-nat-traversal-works/" rel="nofollow"><font style="vertical-align: inherit;">NAT 遍历</font></a><font style="vertical-align: inherit;">。</font></font><a href="https://www.wireguard.com/" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font><a href="https://tailscale.com/blog/how-tailscale-works/" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font><a href="https://tailscale.com/blog/how-nat-traversal-works/" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Tailscale 中的所有内容都是开源的，除了专有操作系统（Windows 和 macOS/iOS）的 GUI 客户端以及控制服务器。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">控制服务器充当 Tailscale 网络中节点的 Wireguard 公钥交换点。</font><font style="vertical-align: inherit;">它分配客户端的 IP 地址，创建每个用户之间的边界，启用用户之间的共享计算机，并公开节点的通告路由。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Tailscale网络</font></font><a href="https://tailscale.com/kb/1136/tailnet/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（tailnet）</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是 Tailscale 以私人用户或组织的方式分配给用户的私有网络。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">设计目标</font></font></h2><a id="user-content-design-goal" class="anchor" aria-label="永久链接：设计目标" href="#design-goal"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Headscale 旨在实现 Tailscale 控制服务器的自托管、开源替代方案。</font><font style="vertical-align: inherit;">Headscale 的目标是为自托管者和爱好者提供可用于其项目和实验室的开源服务器。</font><font style="vertical-align: inherit;">它实现了一个狭窄的范围，一个单一的 Tailnet，适合个人使用，或小型开源组织。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支撑头秤</font></font></h2><a id="user-content-supporting-headscale" class="anchor" aria-label="永久链接：支撑头秤" href="#supporting-headscale"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您喜欢</font></font><code>headscale</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并且发现它有用，存储库中提供了赞助和捐赠按钮。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">特征</font></font></h2><a id="user-content-features" class="anchor" aria-label="永久链接：特点" href="#features"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对 Tailscale 功能的全面“基础”支持</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可配置的DNS
</font></font><ul dir="auto">
<li><a href="https://tailscale.com/kb/1054/dns/#using-dns-settings-in-the-admin-console" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">拆分 DNS</font></font></a></li>
</ul>
</li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">节点注册
</font></font><ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单点登录（通过 Open ID Connect）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">预验证密钥</font></font></li>
</ul>
</li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Taildrop（文件共享）</font></font></li>
<li><a href="https://tailscale.com/kb/1018/acls/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">访问控制列表</font></font></a></li>
<li><a href="https://tailscale.com/kb/1081/magicdns" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">魔法DNS</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持尾网中的多个IP范围</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">双堆栈（IPv4 和 IPv6）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">路由通告（包括出口节点）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">临时节点</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">嵌入式</font></font><a href="https://tailscale.com/blog/how-tailscale-works/#encrypted-tcp-relays-derp" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">DERP服务器</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">客户端操作系统支持</font></font></h2><a id="user-content-client-os-support" class="anchor" aria-label="永久链接：客户端操作系统支持" href="#client-os-support"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">操作系统</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持头秤</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Linux</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是的</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开放BSD</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是的</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自由BSD</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是的</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">苹果系统</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是（请参阅</font></font><code>/apple</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您的头秤以了解更多信息）</font></font></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视窗</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是的</font></font><a href="/juanfont/headscale/blob/main/docs/windows-client.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档</font></font></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安卓</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是的</font></font><a href="/juanfont/headscale/blob/main/docs/android-client.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档</font></font></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">iOS系统</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是的</font></font><a href="/juanfont/headscale/blob/main/docs/iOS-client.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档</font></font></a></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">跑步头秤</font></font></h2><a id="user-content-running-headscale" class="anchor" aria-label="永久链接：跑步头秤" href="#running-headscale"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，我们不支持也不鼓励使用反向代理和容器来运行 Headscale。</font></font></strong></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请看一下</font></font><a href="https://headscale.net/" rel="nofollow"><code>documentation</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">会谈</font></font></h2><a id="user-content-talks" class="anchor" aria-label="永久链接：会谈" href="#talks"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Fosdem 2023（视频）：</font></font><a href="https://fosdem.org/2023/schedule/event/goheadscale/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Headscale：我们如何使用集成测试来重新实现 Tailscale</font></font></a>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">由胡安·丰特·阿隆索和克里斯托弗·达尔比提出</font></font></li>
</ul>
</li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">免责声明</font></font></h2><a id="user-content-disclaimer" class="anchor" aria-label="永久链接：免责声明" href="#disclaimer"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该项目与 Tailscale Inc. 无关。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Headscale 的目的是维护一个工作的、自托管的 Tailscale 控制面板。</font></font></li>
</ol>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贡献</font></font></h2><a id="user-content-contributing" class="anchor" aria-label="永久链接：贡献" href="#contributing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Headscale 是“开源、公认的贡献”，这意味着任何贡献在提交之前都必须与维护者进行讨论。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">选择该模型是为了通过限制审查和验证第三方代码的维护开销来降低倦怠风险。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Headscale 对错误修复的代码贡献持开放态度，无需讨论。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您在文档中发现错误，请提交对文档的修复。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要求</font></font></h3><a id="user-content-requirements" class="anchor" aria-label="永久链接：要求" href="#requirements"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要为 headscale 做出贡献，您需要最新版本的</font></font><a href="https://golang.org" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Go</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
和</font></font><a href="https://buf.build" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Buf</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（Protobuf 生成器）。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们建议使用</font></font><a href="https://nixos.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Nix</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">来设置开发环境。</font><font style="vertical-align: inherit;">这可以通过 来完成</font></font><code>nix develop</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，它将安装工具并为您提供一个 shell。</font><font style="vertical-align: inherit;">这保证了您将拥有与维护者相同的开发环境</font></font><code>headscale</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码风格</font></font></h3><a id="user-content-code-style" class="anchor" aria-label="永久链接：代码风格" href="#code-style"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为了确保我们与越来越多的贡献保持一定的一致性，该项目采用了 linting 和样式/格式规则：</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Go</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码使用</font><font style="vertical-align: inherit;">(width 88) 和
进行</font><font style="vertical-align: inherit;">linted</font></font><a href="https://golangci-lint.run" rel="nofollow"><code>golangci-lint</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和格式化</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">请配置您的编辑器以在开发时运行这些工具，并确保在提交任何代码之前运行这些</font><font style="vertical-align: inherit;">工具</font><font style="vertical-align: inherit;">。</font></font><a href="https://github.com/segmentio/golines"><code>golines</code></a><font style="vertical-align: inherit;"></font><a href="https://github.com/mvdan/gofumpt"><code>gofumpt</code></a><font style="vertical-align: inherit;"></font><code>make lint</code><font style="vertical-align: inherit;"></font><code>make fmt</code><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Proto</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码</font><font style="vertical-align: inherit;">使用 lint</font></font><a href="https://docs.buf.build/lint/overview" rel="nofollow"><code>buf</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和 进行格式化</font></font><a href="https://clang.llvm.org/docs/ClangFormat.html" rel="nofollow"><code>clang-format</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其余</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（Markdown、YAML 等）采用</font></font><a href="https://prettier.io" rel="nofollow"><code>prettier</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">查看</font></font><code>.golangci.yaml</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>Makefile</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">查看具体配置。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装开发工具</font></font></h3><a id="user-content-install-development-tools" class="anchor" aria-label="永久链接：安装开发工具" href="#install-development-tools"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">去</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">缓冲液</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Protobuf工具</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装并激活：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>nix develop</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="nix develop" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">测试和构建</font></font></h3><a id="user-content-testing-and-building" class="anchor" aria-label="永久链接：测试和构建" href="#testing-and-building"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目的某些部分需要从 Protobuf 生成 Go 代码（如果在 中进行了更改</font></font><code>proto/</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">），并且必须使用以下命令（重新）生成：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make generate</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make generate" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：请在单独的提交中签入更改</font></font><code>gen/</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，以便于审查。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行测试：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make <span class="pl-c1">test</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make test" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">构建程序：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>nix build</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="nix build" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或者</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>make build</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="make build" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贡献者</font></font></h2><a id="user-content-contributors" class="anchor" aria-label="永久链接：贡献者" href="#contributors"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<tbody><tr>
    <td align="center">
        <a href="https://github.com/kradalby">
            <img src="https://avatars.githubusercontent.com/u/98431?v=4" width="100;" alt="克里斯托弗" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">克里斯托弗·多尔比</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/juanfont">
            <img src="https://avatars.githubusercontent.com/u/181059?v=4" width="100;" alt="胡安" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胡安·方特</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/restanrm">
            <img src="https://avatars.githubusercontent.com/u/4344371?v=4" width="100;" alt="阿德里安" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿德里安·拉芬·卡布伊斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/cure">
            <img src="https://avatars.githubusercontent.com/u/149135?v=4" width="100;" alt="沃德" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">沃德·范德维奇</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/huskyii">
            <img src="https://avatars.githubusercontent.com/u/5499746?v=4" width="100;" alt="蒋" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">江珠</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/tsujamin">
            <img src="https://avatars.githubusercontent.com/u/2435619?v=4" width="100;" alt="本杰明" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">本杰明·罗伯茨</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/reynico">
            <img src="https://avatars.githubusercontent.com/u/715768?v=4" width="100;" alt="尼科/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">尼科</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/evenh">
            <img src="https://avatars.githubusercontent.com/u/2701536?v=4" width="100;" alt="甚至" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">甚至霍尔特</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/e-zk">
            <img src="https://avatars.githubusercontent.com/u/58356365?v=4" width="100;" alt="e-zk/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">电子ZK</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ImpostorKeanu">
            <img src="https://avatars.githubusercontent.com/u/11574161?v=4" width="100;" alt="贾斯汀" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贾斯汀·安吉尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ItalyPaleAle">
            <img src="https://avatars.githubusercontent.com/u/43508?v=4" width="100;" alt="亚历山德罗" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">亚历山德罗·塞加拉</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ohdearaugustin">
            <img src="https://avatars.githubusercontent.com/u/14001491?v=4" width="100;" alt="哦亲爱的奥古斯丁/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">奥代亚奥古斯丁</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/mpldr">
            <img src="https://avatars.githubusercontent.com/u/33086936?v=4" width="100;" alt="莫里茨" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">莫里茨·波德拉克</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/Orhideous">
            <img src="https://avatars.githubusercontent.com/u/2265184?v=4" width="100;" alt="安德烈" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安德烈·库什尼尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/GrigoriyMikhalkin">
            <img src="https://avatars.githubusercontent.com/u/3637857?v=4" width="100;" alt="格里戈里·米哈尔金/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">格里戈里·米哈尔金</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/christian-heusel">
            <img src="https://avatars.githubusercontent.com/u/26827864?v=4" width="100;" alt="基督教" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">克里斯蒂安·霍塞尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/mike-lloyd03">
            <img src="https://avatars.githubusercontent.com/u/49411532?v=4" width="100;" alt="麦克风" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">迈克·劳埃德</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/iSchluff">
            <img src="https://avatars.githubusercontent.com/u/1429641?v=4" width="100;" alt="安东" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安东·舒伯特</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/Niek">
            <img src="https://avatars.githubusercontent.com/u/213140?v=4" width="100;" alt="尼克" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">尼克·范德马斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/negbie">
            <img src="https://avatars.githubusercontent.com/u/20154956?v=4" width="100;" alt="欧根" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">尤金·比格勒</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/617a7a">
            <img src="https://avatars.githubusercontent.com/u/67651251?v=4" width="100;" alt="阿兹/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿兹</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/qbit">
            <img src="https://avatars.githubusercontent.com/u/68368?v=4" width="100;" alt="亚伦" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">亚伦比伯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/kazauwa">
            <img src="https://avatars.githubusercontent.com/u/12330159?v=4" width="100;" alt="伊戈尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">伊戈尔·佩列皮利岑</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/Aluxima">
            <img src="https://avatars.githubusercontent.com/u/16262531?v=4" width="100;" alt="洛朗" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">洛朗·马绍德</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/majst01">
            <img src="https://avatars.githubusercontent.com/u/410110?v=4" width="100;" alt="斯特凡" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">斯特凡·马耶尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/fdelucchijr">
            <img src="https://avatars.githubusercontent.com/u/69133647?v=4" width="100;" alt="费尔南多" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">费尔南多·德卢基</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/OrvilleQ">
            <img src="https://avatars.githubusercontent.com/u/21377465?v=4" width="100;" alt="奥维尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">奥维尔·宋</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/hdhoang">
            <img src="https://avatars.githubusercontent.com/u/12537?v=4" width="100;" alt="hdhoang/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">赫多昂</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/bravechamp">
            <img src="https://avatars.githubusercontent.com/u/48980452?v=4" width="100;" alt="勇敢冠军/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">布雷尚</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/deonthomasgy">
            <img src="https://avatars.githubusercontent.com/u/150036?v=4" width="100;" alt="德翁" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">德翁·托马斯</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/madjam002">
            <img src="https://avatars.githubusercontent.com/u/679137?v=4" width="100;" alt="杰米" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">杰米·格里夫</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/jonathanspw">
            <img src="https://avatars.githubusercontent.com/u/8390543?v=4" width="100;" alt="乔纳森" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">乔纳森·赖特</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ChibangLW">
            <img src="https://avatars.githubusercontent.com/u/22293464?v=4" width="100;" alt="赤邦LW/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">赤邦LW</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/majabojarska">
            <img src="https://avatars.githubusercontent.com/u/33836570?v=4" width="100;" alt="马哈" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">玛雅·博贾斯卡</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/mevansam">
            <img src="https://avatars.githubusercontent.com/u/403630?v=4" width="100;" alt="梅文" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">梅万·萨马拉通加</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/dragetd">
            <img src="https://avatars.githubusercontent.com/u/3639577?v=4" width="100;" alt="迈克尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">迈克尔·G.</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/ptman">
            <img src="https://avatars.githubusercontent.com/u/24669?v=4" width="100;" alt="保罗" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">保罗·托特曼</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/samson4649">
            <img src="https://avatars.githubusercontent.com/u/12725953?v=4" width="100;" alt="塞缪尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">塞缪尔·洛克</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/loprima-l">
            <img src="https://avatars.githubusercontent.com/u/69201633?v=4" width="100;" alt="洛普马-l/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">洛普马-l</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/unreality">
            <img src="https://avatars.githubusercontent.com/u/352522?v=4" width="100;" alt="不真实/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不真实</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/vsychov">
            <img src="https://avatars.githubusercontent.com/u/2186303?v=4" width="100;" alt="迈克尔·柯/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">迈克尔·柯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/kevin1sMe">
            <img src="https://avatars.githubusercontent.com/u/6886076?v=4" width="100;" alt="凯文林/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">凯文林</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/QZAiXH">
            <img src="https://avatars.githubusercontent.com/u/23068780?v=4" width="100;" alt="小吃/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">小吃</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/artemklevtsov">
            <img src="https://avatars.githubusercontent.com/u/603798?v=4" width="100;" alt="阿尔乔姆" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿乔姆·克莱夫佐夫</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/cmars">
            <img src="https://avatars.githubusercontent.com/u/23741?v=4" width="100;" alt="凯西" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">凯西·马歇尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/dbevacqua">
            <img src="https://avatars.githubusercontent.com/u/6534306?v=4" width="100;" alt="德贝瓦夸/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">德贝瓦夸</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/joshuataylor">
            <img src="https://avatars.githubusercontent.com/u/225131?v=4" width="100;" alt="乔什" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">乔什·泰勒</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/CNLHC">
            <img src="https://avatars.githubusercontent.com/u/21005146?v=4" width="100;" alt="刘" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">刘汉成</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/motiejus">
            <img src="https://avatars.githubusercontent.com/u/107720?v=4" width="100;" alt="莫蒂尤斯" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">莫泰尤斯·杰克斯蒂斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/pvinis">
            <img src="https://avatars.githubusercontent.com/u/100233?v=4" width="100;" alt="帕夫洛斯" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">帕夫洛斯·维涅拉托斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/SilverBut">
            <img src="https://avatars.githubusercontent.com/u/6560655?v=4" width="100;" alt="银" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">银子弹</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/snh">
            <img src="https://avatars.githubusercontent.com/u/2051768?v=4" width="100;" alt="史蒂文" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">史蒂文·洪森</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ratsclub">
            <img src="https://avatars.githubusercontent.com/u/25647735?v=4" width="100;" alt="胜利者" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">维克托·弗莱雷</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/qzydustin">
            <img src="https://avatars.githubusercontent.com/u/44362429?v=4" width="100;" alt="振宇" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">齐振宇</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/t56k">
            <img src="https://avatars.githubusercontent.com/u/12165422?v=4" width="100;" alt="托马斯/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">托马斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/puzpuzpuz">
            <img src="https://avatars.githubusercontent.com/u/37772591?v=4" width="100;" alt="安德烈" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安德烈·佩奇库洛夫</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/linsomniac">
            <img src="https://avatars.githubusercontent.com/u/466380?v=4" width="100;" alt="肖恩" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">肖恩·赖夫施奈德</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/aberoham">
            <img src="https://avatars.githubusercontent.com/u/586805?v=4" width="100;" alt="亚伯拉罕" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">亚伯拉罕·英格索尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/iFargle">
            <img src="https://avatars.githubusercontent.com/u/124551390?v=4" width="100;" alt="阿尔伯特" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿尔伯特·科普兰</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/theryecatcher">
            <img src="https://avatars.githubusercontent.com/u/16442416?v=4" width="100;" alt="阿努普" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿努普·桑达雷什</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/apognu">
            <img src="https://avatars.githubusercontent.com/u/3017182?v=4" width="100;" alt="安托万" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安托万·波波诺</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/tony1661">
            <img src="https://avatars.githubusercontent.com/u/5287266?v=4" width="100;" alt="安东尼奥" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安东尼奥·费尔南德斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/aofei">
            <img src="https://avatars.githubusercontent.com/u/5037285?v=4" width="100;" alt="奥飞" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">奥飞盛</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/arnarg">
            <img src="https://avatars.githubusercontent.com/u/1291396?v=4" width="100;" alt="阿尔纳尔/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿尔纳尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/awoimbee">
            <img src="https://avatars.githubusercontent.com/u/22431493?v=4" width="100;" alt="亚瑟" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">亚瑟·沃因比</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/avirut">
            <img src="https://avatars.githubusercontent.com/u/27095602?v=4" width="100;" alt="阿维鲁特" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿维鲁特·梅塔</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/winterheart">
            <img src="https://avatars.githubusercontent.com/u/81112?v=4" width="100;" alt="阿扎马特" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿扎马特·H·哈基莫夫</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/stensonb">
            <img src="https://avatars.githubusercontent.com/u/933389?v=4" width="100;" alt="布莱恩" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">布莱恩·斯滕森</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/yangchuansheng">
            <img src="https://avatars.githubusercontent.com/u/15308462?v=4" width="100;" alt="卡森" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">杨卡森</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/kundel">
            <img src="https://avatars.githubusercontent.com/u/10158899?v=4" width="100;" alt="达雷尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">达雷尔·昆德尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/fatih-acar">
            <img src="https://avatars.githubusercontent.com/u/15028881?v=4" width="100;" alt="法提赫-阿卡尔/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">法蒂赫阿卡尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/fkr">
            <img src="https://avatars.githubusercontent.com/u/51063?v=4" width="100;" alt="菲利克斯" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">菲利克斯·克罗拉格-达默斯</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/felixonmars">
            <img src="https://avatars.githubusercontent.com/u/1006477?v=4" width="100;" alt="菲利克斯" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">严菲利克斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/gabe565">
            <img src="https://avatars.githubusercontent.com/u/7717888?v=4" width="100;" alt="加布" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">加布·库克</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/JJGadgets">
            <img src="https://avatars.githubusercontent.com/u/5709019?v=4" width="100;" alt="JJ小工具/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">JJ小玩意</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/hrtkpf">
            <img src="https://avatars.githubusercontent.com/u/42646788?v=4" width="100;" alt="hrtkpf/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">心率</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/jessebot">
            <img src="https://avatars.githubusercontent.com/u/2389292?v=4" width="100;" alt="杰西机器人/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">杰西博特</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/jimt">
            <img src="https://avatars.githubusercontent.com/u/180326?v=4" width="100;" alt="吉姆" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">吉姆·蒂茨勒</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/jsiebens">
            <img src="https://avatars.githubusercontent.com/u/499769?v=4" width="100;" alt="约翰" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">约翰·西本斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/johnae">
            <img src="https://avatars.githubusercontent.com/u/28332?v=4" width="100;" alt="约翰" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">约翰·阿克塞尔·埃里克森</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ShadowJonathan">
            <img src="https://avatars.githubusercontent.com/u/22740616?v=4" width="100;" alt="乔纳森" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">乔纳森·德容</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/JulienFloris">
            <img src="https://avatars.githubusercontent.com/u/20380255?v=4" width="100;" alt="朱利安" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">朱利安·兹维林克</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/win-t">
            <img src="https://avatars.githubusercontent.com/u/1589120?v=4" width="100;" alt="库尼亚" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">库尼亚·D·温</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/Lucalux">
            <img src="https://avatars.githubusercontent.com/u/70356955?v=4" width="100;" alt="卢卡卢克斯/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">卢卡卢克斯</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/foxtrot">
            <img src="https://avatars.githubusercontent.com/u/4153572?v=4" width="100;" alt="马克/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">马克</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/mhameed">
            <img src="https://avatars.githubusercontent.com/u/447017?v=4" width="100;" alt="梅萨尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">梅萨尔·哈米德</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/mikejsavage">
            <img src="https://avatars.githubusercontent.com/u/579299?v=4" width="100;" alt="迈克尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">迈克尔·萨维奇</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/pkrivanec">
            <img src="https://avatars.githubusercontent.com/u/25530641?v=4" width="100;" alt="菲利普" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">菲利普·克里瓦内克</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/piec">
            <img src="https://avatars.githubusercontent.com/u/781471?v=4" width="100;" alt="皮埃尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">皮埃尔·卡鲁</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/donran">
            <img src="https://avatars.githubusercontent.com/u/4838348?v=4" width="100;" alt="本都" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">本都 N</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/nnsee">
            <img src="https://avatars.githubusercontent.com/u/36747857?v=4" width="100;" alt="拉斯穆斯" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">拉斯穆斯·穆拉特</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/rcursaru">
            <img src="https://avatars.githubusercontent.com/u/16259641?v=4" width="100;" alt="库尔萨鲁/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">鲁库尔萨鲁</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/renovate-bot">
            <img src="https://avatars.githubusercontent.com/u/25180681?v=4" width="100;" alt="修补" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">修补翻新</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ryanfowler">
            <img src="https://avatars.githubusercontent.com/u/2668821?v=4" width="100;" alt="瑞安" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">瑞恩·福勒</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/muzy">
            <img src="https://avatars.githubusercontent.com/u/321723?v=4" width="100;" alt="塞巴斯蒂安/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">塞巴斯蒂安</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/shaananc">
            <img src="https://avatars.githubusercontent.com/u/2287839?v=4" width="100;" alt="沙南" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">沙南·科尼</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/6ixfalls">
            <img src="https://avatars.githubusercontent.com/u/23470032?v=4" width="100;" alt="六/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">六</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/stefanvanburen">
            <img src="https://avatars.githubusercontent.com/u/622527?v=4" width="100;" alt="斯特凡" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">斯特凡·范布伦</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/sophware">
            <img src="https://avatars.githubusercontent.com/u/41669?v=4" width="100;" alt="软件/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">软件</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/m-tanner-dev0">
            <img src="https://avatars.githubusercontent.com/u/97977342?v=4" width="100;" alt="皮匠/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">皮匠</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/Teteros">
            <img src="https://avatars.githubusercontent.com/u/5067989?v=4" width="100;" alt="泰特罗斯/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">泰特罗斯</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/gitter-badger">
            <img src="https://avatars.githubusercontent.com/u/8518239?v=4" width="100;" alt="这" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">吉特獾</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/tianon">
            <img src="https://avatars.githubusercontent.com/u/161631?v=4" width="100;" alt="天农" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">天农重力</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/thetillhoff">
            <img src="https://avatars.githubusercontent.com/u/25052289?v=4" width="100;" alt="直到" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">蒂尔·霍夫曼</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/woudsma">
            <img src="https://avatars.githubusercontent.com/u/6162978?v=4" width="100;" alt="提尔克" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提尔克·沃兹玛</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/y0ngb1n">
            <img src="https://avatars.githubusercontent.com/u/25719408?v=4" width="100;" alt="杨斌" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">杨斌阿本</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/sleepymole">
            <img src="https://avatars.githubusercontent.com/u/17199941?v=4" width="100;" alt="玉杰" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">夏玉杰</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/newellz2">
            <img src="https://avatars.githubusercontent.com/u/52436542?v=4" width="100;" alt="扎卡里" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">扎卡里·纽厄尔</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/zekker6">
            <img src="https://avatars.githubusercontent.com/u/1367798?v=4" width="100;" alt="扎哈尔" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">扎哈尔·贝萨拉布</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/zhzy0077">
            <img src="https://avatars.githubusercontent.com/u/8717471?v=4" width="100;" alt="致远" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">郑志远</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/Bpazy">
            <img src="https://avatars.githubusercontent.com/u/9838749?v=4" width="100;" alt="紫苑" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">韩子元</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/caelansar">
            <img src="https://avatars.githubusercontent.com/u/31852257?v=4" width="100;" alt="凯兰萨尔/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">凯兰萨尔</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/derelm">
            <img src="https://avatars.githubusercontent.com/u/465155?v=4" width="100;" alt="德雷姆/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">德雷姆</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/dnaq">
            <img src="https://avatars.githubusercontent.com/u/1299717?v=4" width="100;" alt="DNAq/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">脱氧核糖核酸</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/nning">
            <img src="https://avatars.githubusercontent.com/u/557430?v=4" width="100;" alt="亨宁" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">亨宁·米勒</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ignoramous">
            <img src="https://avatars.githubusercontent.com/u/852289?v=4" width="100;" alt="无知/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无知的</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/jimyag">
            <img src="https://avatars.githubusercontent.com/u/69233189?v=4" width="100;" alt="吉米亚格/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">吉米亚格</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/magichuihui">
            <img src="https://avatars.githubusercontent.com/u/10866198?v=4" width="100;" alt="苏海伦/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">苏海伦</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/lion24">
            <img src="https://avatars.githubusercontent.com/u/1382102?v=4" width="100;" alt="鲨鱼网/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">鲨鱼网</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/ma6174">
            <img src="https://avatars.githubusercontent.com/u/1449133?v=4" width="100;" alt="ma6174/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">马6174</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/manju-rn">
            <img src="https://avatars.githubusercontent.com/u/26291847?v=4" width="100;" alt="文殊-rn/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文殊菩萨</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/nicholas-yap">
            <img src="https://avatars.githubusercontent.com/u/38109533?v=4" width="100;" alt="尼古拉斯·雅普/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">尼古拉斯·亚普</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/pernila">
            <img src="https://avatars.githubusercontent.com/u/12460060?v=4" width="100;" alt="托米" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">托米·佩尼拉</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/phpmalik">
            <img src="https://avatars.githubusercontent.com/u/26834645?v=4" width="100;" alt="phpmalik/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">phpmalik</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/Wakeful-Cloud">
            <img src="https://avatars.githubusercontent.com/u/38930607?v=4" width="100;" alt="清醒的" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">醒云</font></font></b></sub>
        </a>
    </td>
    <td align="center">
        <a href="https://github.com/xpzouying">
            <img src="https://avatars.githubusercontent.com/u/3946563?v=4" width="100;" alt="兹/" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">兹</font></font></b></sub>
        </a>
    </td>
</tr>
<tr>
    <td align="center">
        <a href="https://github.com/atorregrosa-smd">
            <img src="https://avatars.githubusercontent.com/u/78434679?v=4" width="100;" alt="埃莱克斯" style="max-width: 100%;">
            <br>
            <sub><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">艾莱克斯·托雷格罗萨</font></font></b></sub>
        </a>
    </td>
</tr>
</tbody></table>
</article></div>
