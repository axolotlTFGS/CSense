# CSense 常见问题

因不慎揭露真相，我们的官方账户遭到了官方开发人员及社区扩展开发者的猛烈批判，且官方以莫须有之罪立刻封禁了我们的官方 CCW 账户。故，我们现在将未审查的版本置于 GitHub，以确保所有人都能了解到真相。同时，我们会为每个回答尽可能添加证据。

---

> 你们的目的是什么？

A：我们的目的在 GitHub README 已经说明。具体请参照 https://github.com/axolotlTFGS/CSense 。目前我们的行动暂没有取得任何进展，怀疑可能是官方优越感过强所致。

---

> 你们是谁？

A：无可奉告，然而 CSense 的其中一位主力开发者曾经发布过《TFGS》和《求精华》等作品，希望可以成为开户我们的大概依据。

---

> 唐豆和你们什么关系？

A：唐豆是我们的美工。目前，他已经宣布退出 CSense 团队。他没有获得任何 CSense 的源代码。

---

> 为什么要破坏公益社区？

A：并非公益。CCW 不是非营利性组织[1]。根据企查查及共创世界官方开展的部分活动推测，他们通过建立同政府及教育机构的合作[2]、吸引风险投资，以及向网课机构引流/反哺来获得利益。然而，即使是在号称“大爆料”的最新发布的 CCW QA 中，社区运维仍然在这一点上转移话题，含糊其辞。
延伸思考：Steam “香蕉游戏”是如何获得利益的？

相关引用及证据：
1. 企查查页面：https://www.qcc.com/firm/22bfa10d8af4ee24ab7f890823d32d0b.html
2. 官方同中国电子学会合作：https://learn.ccw.site/article/news/cdddc946-b7d4-427b-9451-fda8c7695533

---

> 为什么要破坏以热爱面对挑战的热情？

A：并非热爱。根据 Gandi IDE 开源的源代码和提交记录可知，Gandi IDE 官方开发者对用户建议 [3] 及安全漏洞 [来源请求] 响应不及时，同时在开发中存在玩忽职守、经验不足 [1]、消极开源（注：在有能力的情况下未向上游反哺任何代码）、过于急躁、代码质量不合格 [2] 等众多问题，
如无视 eslint 警告在源代码中使用最差实践 [2]。根据社区调查，Gandi IDE 官方开发者几乎都为兼职 [4]，且对 CSense 公布安全漏洞引起的讨论持消极态度 [5]。如果官方开发者真正热爱 Scratch，我们认为 CSense 也没有存在的意义了。

相关引用及证据：
1. 你猜为什么我们挂那么多 tag 还能发出去呢？
2. 如 https://github.com/Gandi-IDE/scratch-vm/blob/develop/src/extension-support/extension-manager.js#L103 的 `isConstructor` 函数存在性能问题并违反 eslint 规则，且可以被以下代码轻易重构（数据来源 https://github.com/Gandi-IDE/scratch-vm/pull/7 ）：
```
const isConstructor = value => !!value.prototype;
```
然而，截至 commit `7b3e5b56ce9006112188d0172dee252f8e080c71`，有问题的代码仍然没有被更正。  

3. https://github.com/Gandi-IDE/scratch-vm/pull/3  
4. 来自 sylarhcn 于“Gandi 内部开发群”的发言。消息渠道保密。  
5. 来自 sylarhcn 于“Gandi 内部开发群”对于 CSense 的评论。消息渠道保密。  
![image](https://github.com/user-attachments/assets/5ca420d0-919c-4888-888b-6853a045a190)

---

> 你们如何看待最近的外挂盛行？

A：这是社区风气问题。根据调查，在阿尔法营和 ClipCC 社区，即使已有部分用户发布了盗取源代码 [1]、下载作品，或者作弊的简易方式，这些社区的同平台盗作/作弊情况仍然罕见，且社区用户对于此类工具大多持反对态度。然而，CSense 一经发布即遭到严重的非法滥用 [2]，一度影响热门作品的正常使用，其背后的原因想必不难推测。
社区的风气一定程度上由官方的风气决定，如果 CCW 在创立之初没有使用水军向阿尔法营大量发送引流广告 [3]，想必 CCW 今日的社区风气应当和其它社区持平。

相关引用及证据：
1. https://github.com/hite4044/ClipCC-Project-Downloader
2. 触不可及
3. 证据来自阿尔法营交流群

---

> 你们这么做良心不会痛么？

A：Gandi IDE 开发者在挪用 [1] TurboWarp 源代码而不注明 TurboWarp [2]，导致大部分用户甚至不知道 Gandi IDE 基于 TurboWarp 源代码时；或者扩展集市允许自由上传而导致 TurboWarp 扩展被用户未经原作者允许而违反开源许可证上传到 Gandi IDE 时 [3]，他们的良心也没有痛过。

相关引用及证据：
1. 以下给出一个例子。
https://github.com/Gandi-IDE/scratch-vm/blob/develop/src/extension-support/tw-security-manager.js 和 https://github.com/TurboWarp/scratch-vm/blob/develop/src/extension-support/tw-security-manager.js 的内容惊人地相似。
如果如同多 bug 的哮天犬于 https://learn.ccw.site/article/dda700ce-ee4d-46c4-a7c6-e8a52a516b1c 中的发言一致（“这里我要声明一点，Gandi IDE是重写了TW的代码！不是Fork！”），这会让我们不禁想起[甲骨文诉谷歌Java侵权案](https://zh.wikipedia.org/wiki/%E7%94%B2%E9%AA%A8%E6%96%87%E8%AF%89%E8%B0%B7%E6%AD%8CJava%E4%BE%B5%E6%9D%83%E6%A1%88)，以及 [CEC-IDE](https://www.163.com/dy/article/ID3R33830511D6RL.html) 的事情来。
2. https://getgandi.com/cn 中，有如下一段：
```
Q：Gandi IDE 是开源的吗？
A：是的，Gandi IDE 是一个基于 LLK/Scratch 开发的 Scratch 编辑器。使用到的开源库与开源代码，可以在 IDE 的设置菜单中查看详情。
```
此处没有提到对 TurboWarp 代码的使用。
相比 Gandi IDE 的 GitHub 仓库来说，显然这个 URL 更加广为人知。

3. https://assets.ccw.site/extension/snowiceJSON https://assets.ccw.site/extension/some58358 https://assets.ccw.site/extension/Cast https://assets.ccw.site/extension/HideBlock https://assets.ccw.site/extension/fetch https://assets.ccw.site/extension/lmsHackedBlocks https://assets.ccw.site/extension/jeremygamerTweening https://assets.ccw.site/extension/skyhigh173JSON https://assets.ccw.site/extension/controlkj https://assets.ccw.site/extension/shovelcss https://assets.ccw.site/extension/xeltallivSimple3D https://assets.ccw.site/extension/shovellzcompress https://assets.ccw.site/extension/pointerlock https://assets.ccw.site/extension/nkcontrols https://assets.ccw.site/extension/clipboard https://assets.ccw.site/extension/localstorage https://assets.ccw.site/extension/lmsTimers https://assets.ccw.site/extension/battery2.0 https://assets.ccw.site/extension/cubesterWindowControls https://assets.ccw.site/extension/mdwaltersnotifications https://assets.ccw.site/extension/alestorenfc https://assets.ccw.site/extension/numericalencoding2 这些扩展都是用户上传的，但官方没有采取任何措施防止这样的行为（和 CSense 不采取任何措施防止脚本小子一样）。
---

> 为什么 CSense 不设置门槛让脚本小子不能使用？

A：因为脚本小子在向扩展集市上传 TurboWarp 扩展时也没有门槛。关于扩展集市不审核/差别审核的问题，TurboWarp 社区曾经因熊谷 凌当传话太监而一度传来怨言 [1]，当时 Gandi IDE 社区扩展开发者将 TurboWarp 频道变为了互相人身攻击和抹黑的论战 [1]。当时开发者曾经承诺会上线严格的审核机制并第一时间移除侵犯著作权的内容，然而此次承诺随后不了了之，在最新的 CCW QA 中，我们没有看到任何关于扩展集市审核机制的日程安排，也没有任何关于这一点的具体问题 [2]。
让我们换一个角度。我们不希望限制任何用户使用 CSense 的自由，特别是在考虑到这样做的后果不及 CCW 官方决策后果的情况下。

相关引用及证据：
1. 原讨论于 TurboWarp Discord 服务器的 #off-topic-and-memes 频道中。
2. 参见 https://learn.ccw.site/article/fac7781b-deb1-48e6-bad9-2a8ddf358ca9。

---

> CSense 怎么时常加载不出来啊？

A：目前我们的运行环境已经全面由篡改猴转移到暴力猴以解决一些运行环境带来的问题，因此删除篡改猴而下载暴力猴可能会解决这种问题。此外，多次刷新页面、打开开发者工具，以及重新登录都有助于解决此问题。

---

> 我发现你们帮助 CCW 修复了一些安全漏洞。你们会考虑向 CCW 官方共享这些代码么？

A：在我们达到目的以前，我们不会主动与官方合作。我们永远不会向他们共享我们的源代码和未来可能收集的用户数据。

---

> CSense 会盗号或者添加后门么？

A：由于 token 目前已经被标记为 HttpOnly，因此我们无法访问您的 token，您也无需担心账号被盗。此外，添加后门需要远程服务器，我们不希望增加这种没有意义的开发成本。

---

> 主播，我怎么不能在 Nostalgist 里面开挂啊？

A：我们没有时间和精力去专门为一个更改存档就可以实现作弊的套壳作品设计调试功能，也不关心任何主要实现部分不在 Scratch 的作品。

---

> 官方有办法追回我的损失么？/我有办法转走共创币而不被封号？

A：官方没有办法追回你的损失 [1]，具体原因不再重复叙述。官方开发人员确实可以通过手动还原数据库的方式来恢复您的部分损失，但这样做的人力成本十分大，因此不太可能。如果您希望自己转走的共创币不被撤销，您可以在短时间内将获得的金币快速转移到不同的经济合约或作品投币中，从而避免被封号后无法提取金币。

相关引用及证据：
1. https://learn.ccw.site/article/a374d446-c77b-46a8-9cec-35d8aa6c5f4a 中有以下内容：

> ### 解释
> 关于金币的强制归还
> 官方无权利变动
> 故只能敦促，无法强制
> 最高的处理级别是封号

---

> 触不可及是怎么偷币的？/我如何破解 Gandi IDE 的 AB 摘要？

A：触不可及通过 XSS 脚本（Gandi IDE 自身的漏洞）来伪装成您进行转账操作。此漏洞已经被 CSense 修复，但可能引起性能问题。由于 Gandi IDE 对于关键接口的 AB 摘要是以 axios interceptor 形式实现的，您可以在代码中通过劫持 React 元素来获得 axios 上下文，并使用 axios 发送请求即可通过黑箱的方式绕过此摘要。此外，对于 Gandi Desktop，您可以使用 `window.electron.ipcRenderer.sendSync('auth:get-token')` 获取用户认证信息，具体作用我们不会展开叙述。

---

> 多 bug 的哮天犬怎么急了 (https://learn.ccw.site/article/dda700ce-ee4d-46c4-a7c6-e8a52a516b1c)？

A：不是我们让他急的，我们无能为力。祝他早日修复 CSense 提出的各种安全漏洞。同时，我们能发出那篇文章也侧面说明了共创世界后端的经验不足。
