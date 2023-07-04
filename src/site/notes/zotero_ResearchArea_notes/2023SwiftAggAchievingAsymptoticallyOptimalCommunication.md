---
{"dg-publish":true,"permalink":"/zotero_ResearchArea_notes/2023SwiftAggAchievingAsymptoticallyOptimalCommunication/"}
---


# SwiftAgg+: Achieving Asymptotically Optimal Communication Loads in Secure Aggregation for Federated Learning

## One-sentence summary

## Metadata

>[!info] Info
>- **Title**: SwiftAgg+: Achieving Asymptotically Optimal Communication Loads in Secure Aggregation for Federated Learning 
>- **Author**: Tayyebeh Jahani-Nezhad, Mohammad Ali Maddah-Ali, Songze Li, Giuseppe Caire
>- **Year**: 2023-04-01
>- **Bibliography**: Jahani-Nezhad, T., Maddah-Ali, M. A., Li, S., & Caire, G. (2023). SwiftAgg+: Achieving Asymptotically Optimal Communication Loads in Secure Aggregation for Federated Learning. _IEEE Journal on Selected Areas in Communications_, _41_(4), 977–989. [https://doi.org/10.1109/JSAC.2023.3242702](https://doi.org/10.1109/JSAC.2023.3242702)

> [!abstract] Abstract
> We propose <monospace>SwiftAgg+</monospace>, a novel secure aggregation protocol for federated learning systems, where a central server aggregates local models of <inline-formula> <tex-math notation="LaTeX">$N \in \mathbb {N}$ </tex-math></inline-formula> distributed users, each of size <inline-formula> <tex-math notation="LaTeX">$L \in \mathbb {N}$ </tex-math></inline-formula>, trained on their local data, in a privacy-preserving manner. <monospace>SwiftAgg+</monospace> can significantly reduce the communication overheads without any compromise on security, and achieve optimal communication loads within diminishing gaps. Specifically, in presence of at most <inline-formula> <tex-math notation="LaTeX">$D=o(N)$ </tex-math></inline-formula> dropout users, <monospace>SwiftAgg+</monospace> achieves a per-user communication load of <inline-formula> <tex-math notation="LaTeX">$\left({1+\mathcal {O}\left({\frac {1}{N}}\right)}\right)L$ </tex-math></inline-formula> symbols and a server communication load of <inline-formula> <tex-math notation="LaTeX">$\left({1+\mathcal {O}\left({\frac {1}{N}}\right)}\right)L$ </tex-math></inline-formula> symbols, with a worst-case information-theoretic security guarantee, against any subset of up to <inline-formula> <tex-math notation="LaTeX">$T=o(N)$ </tex-math></inline-formula> semi-honest users who may also collude with the curious server. Moreover, the proposed <monospace>SwiftAgg+</monospace> allows for a flexible trade-off between communication loads and the number of active communication links. In particular, for N<T-D and for any <inline-formula> <tex-math notation="LaTeX">$K\in \mathbb {N}$ </tex-math></inline-formula>, <monospace>SwiftAgg+</monospace> can achieve the server communication load of <inline-formula> <tex-math notation="LaTeX">$\left({1+\frac {T}{K}}\right)L$ </tex-math></inline-formula> symbols, and per-user communication load of up to <inline-formula> <tex-math notation="LaTeX">$\left({1+\frac {T+D}{K}}\right)L$ </tex-math></inline-formula> symbols, where the number of pair-wise active connections in the network is <inline-formula> <tex-math notation="LaTeX">$\frac {N}{2}(K+T+D+1)$ </tex-math></inline-formula>.

> [!example] Files and Links 
>- **DOI**: 10.1109/JSAC.2023.3242702
>- **Url**: https://ieeexplore.ieee.org/document/10058697/
>- **PDF**: [2023_Jahani-Nezhad et al_SwiftAgg+.pdf](file://C:\Users\可可\OneDrive%20-%20sjtu.edu.cn\Zotero\storage\2023IEEE%20Journal%20on%20Selected%20Areas%20in%20Communications\2023_Jahani-Nezhad%20et%20al_SwiftAgg+2.pdf)
>- **Zotero**: [2023_Jahani-Nezhad et al_SwiftAgg+.pdf](zotero://select/library/items/9Y5DQZAI)

> [!tip] Zotero Tags
>- **Keywords**: #unread, #CCF-A

## Annotations


---
# Obsidian Notes
我们提出了 SwiftAgg+，一种用于联邦学习系统的新型安全聚合协议，其中中央服务器聚合N个分布式用户的本地模型，每个模型的大小为L，以隐私保护的方式对其本地数据进行训练。 SwiftAgg+可以在不影响安全性的情况下显着减少通信开销，并实现最佳的通信负载。具体来说，在最多存在 D = O(N) 个dropout用户的情况下，SwiftAgg+ 实现的每个用户的通信负载为 (1 + O( 1/N ))L 个symbols，服务器通信负载为 (1 + O( 1/N ) )L 个symbols，具有最坏情况的信息论安全保证，针对最多 T =O(N) 个半诚实用户的任何子集，这些用户也可能与好奇的服务器勾结。此外，我们提出的 SwiftAgg+ 允许在通信负载和active通信链路数量之间进行灵活的权衡。特别是，对于 T < N − D 且对于任意 K ∈ N，SwiftAgg+ 可以实现 (1 + T/K )L 个符号的服务器通信负载，以及高达 (1 + (T +D)/K )L 个symbols的每用户通信负载，其中网络中pair-wise的active的连接的数量为 N/2 * (K + T + D + 1)。

## 辅助资料

## What can we learn

## Q1 论文试图解决什么问题？

## Q2 这是否是一个新的问题？

作为本手稿的早期会议版本，在 [14] 中，我们提出了 SwiftAgg，它通过将用户划分为多个组并使用 Shamir 的秘密共享 [15] 来保持本地模型的私密性，从而减少服务器通信负载。 SwiftAgg 能够在最多 D 个退出用户的情况下实现正确的聚合，并正式证明针对最多 T 个半诚实用户的最坏情况安全保证。独立地，CodedSecAgg [16] 中也使用了类似的想法，但组中的退出用户尚未得到解决，也没有正式的定义和隐私证明。现有方法的通信负载和计算负载在表1中进行了比较。

![](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230626195503.png)

## Q3 这篇文章要验证一个什么科学假设？

## Q4 有哪些相关研究？如何归类？谁是这一课题在领域内值得关注的研究员？

### SecAgg
请注意，为了具有信息论安全性，必须从大小为 L 的向量中统一随机选择共享和私有随机向量。然而，为了使其在 SecAgg 中实用，假设用户同意伪随机生成器而不是整个共享随机向量，这在信息论的背景下是不安全的。在本文中，我们重点关注信息论安全保证。

SecAgg 扩展的主要挑战之一是通信负载。用户之间的秘密共享需要全对全的通信，这会产生用户数量 N 的二次方成本。已经有一系列旨在提高 SecAgg 通信效率的工作（参见，例如，[7]–[ 9]）。

### （降低通信负载）SecAgg扩展1：TurboAgg
在[7]中，TurboAgg被提出按照**圆形拓扑**执行安全聚合，在服务器处实现O(LN log N)，在每个用户处实现O(L log N)的通信负载。 TurboAgg 的思想是将用户分为几个组，每个组的大小为 O(log N)，以加速模型聚合阶段。为了保护单个模型，每个用户都以特定的方式掩盖其本地模型。此外，2 屏蔽本地模型使用拉格朗日编码计算 [10] 进行编码，以便可以在协议的每个阶段恢复丢失用户的数据。组中的每个用户计算前一组中所有用户的屏蔽模型的聚合和编码模型的聚合，并将其发送给下一组中的所有用户，以及其模型的屏蔽和编码版本。如果组中至少有一半的用户没有退出，则由退出用户引起的聚合屏蔽模型的缺失项可以在下一组中恢复。只要半诚实用户的数量小于 N/2，TurboAgg 就能以高概率保证各个局部模型的隐私。

### （降低通信负载）SecAgg扩展2：SecAgg+
在[8]中，提出了SecAgg+，它考虑用户之间的**k-正则通信图**而不是SecAgg中使用的完整图，以减少通信和计算负载，其中k = O(log N)。这意味着每个用户秘密与其他用户的子集共享，而不是与所有用户共享。结果表明，SecAgg+ 在服务器上需要 O(LN + N log N) 的通信，在每个用户上需要 O(L +log N) 的通信。在[9]中，提出了另一个类似的想法CCESA，其中使用稀疏随机图而不是完整图作为通信网络。因此，秘密共享用于一部分用户而不是全部通信。虽然 SecAgg+、TurboAgg 和 CCESA 提高了 SecAgg 的通信效率，但它们仅提供概率隐私保证，而不是 SecAgg 的最坏情况保证。

### （降低计算复杂性）SecAgg扩展3： FastSecAgg
其他一些安全聚合协议侧重于降低 SecAgg 的计算复杂性，而不是通信负载。 FastSecAgg在[11]中提出，提出了一种**基于快速傅里叶变换的有限域版本的多秘密共享方案**，以实现秘密数量、丢失容忍度和隐私阈值之间的权衡。 FastSecAgg将服务器和每个用户的计算负载降低到O(L log N)，同时实现与SecAgg相同的通信顺序，具有更低的隐私阈值和丢包容忍度。

### （降低计算复杂性）SecAgg扩展4： LightSecAgg
在[12]中，提出了LightSecAgg来减少安全聚合中的计算复杂度瓶颈。在 LightSecAgg 中，每个用户独立采样随机掩码，**使用 T-private MDS（最大距离可分离）编码对其进行编码**，生成掩码的秘密份额以发送给其他用户。然后，每个用户将蒙版添加到其本地模型并将蒙版模型发送到服务器。服务器可以使用在与幸存用户通信的第二阶段中接收到的聚合编码掩码，通过一次性解码来重建并消除幸存用户的聚合掩码。 [13]中也采用了类似的聚合掩码一次性重建的想法，但这需要可信的第三方，并且需要生成更多的随机性，以及每个用户的更多存储空间。
## Q5 论文中提到的解决方案之关键是什么？

###  SwiftAgg+方案概述
在本文中，我们提出 SwiftAgg+ 作为联邦学习中安全聚合的新方案，该方案对于最多 D 个用户dropout具有鲁棒性，并针对最多 T < N − D 个可能与他人或服务器串通以获取信息的半诚实用户实现最坏情况的安全保证。

在 SwiftAgg+ 中，为了以保护隐私的方式计算本地模型的聚合，只要 T = o(N) 且 N -D=O(N)，服务器接收到的符号数量为 (1 + O( 1/N ))L。另外，对于T=o(N)且D=o(N)，每个用户发送的符号数量为(1+O(1/N))L。

此外，由于在联邦学习中许多用户可能无法相互访问，因此用户之间或从用户到服务器的active通信链路的数量也是设计安全聚合协议时的一个重要因素。 SwiftAgg+ 允许在通信负载和网络连接之间进行灵活的权衡。为了实现这种权衡，我们首先将用户划分为大小为 T + D + K 的组，其中 K ∈ N（见图 4），并将这些组排列在以服务器为根的任意分层树上。然后:
1. 在第一阶段，每个用户将其本地模型划分为 K 个部分。
2. 在第二阶段，每个组秘密中的用户使用斜坡秘密共享（ramp secret sharing）[17]共享其本地模型的partitions，并在本地聚合shares。
3. 第三阶段，每个用户聚合in-group shares以及从其children groups中相应用户接收到的消息，并将结果发送给其parent group中相应用户，最后发送到服务器。在第三阶段，如果组中的一个用户退出，则包括该退出用户的sequence中的其余用户保持silent。该聚合树提供了根据网络连接调整训练过程每次迭代的delay的灵活性。此外，参数 K 控制通信负载和网络连接性之间的tradeoff，可以根据网络的约束来选择参数 K。
![](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230627000233.png)

### SwiftAgg+优点
与现有作品相比，SwiftAgg+同时实现了以下优点：
1. 对于 T = o(N) 和 N − D = O(N)，SwiftAgg+ 中的服务器通信负载是within factor 1 of the cut-set lower bound（🤔）。
2. SwiftAgg+ 可以灵活地减少用户之间的活动连接数量，但代价是增加通信负载，使其偏离最佳状态。
3. 它能够适应最多 D 个用户的退出。与现有方案相反，在 SwiftAgg+ 中，由于该方案的结构，用户dropout的影响已经在与服务器的一轮通信中得到处理，无需进行另一轮通信。
4. 它针对好奇的服务器和最多 T < N − D 半诚实用户的任何子集实现了最坏情况的信息论安全性。
5. 基于用户之间可能的连接，SwiftAgg+可以灵活地控制每次训练迭代的delay。

### SwiftAgg+与现有方案对比
表一比较了安全聚合问题的不同方案在通信和计算负载方面的情况。为了公平比较，我们考虑两个指标：服务器通信负载和每用户通信负载。服务器通信负载表示服务器发送或接收的所有消息的聚合大小，每用户通信负载表示每个用户发送的所有消息的聚合大小。此外，服务器和每用户计算分别指示服务器和每个用户的计算负载。在该表中，[7]、[12]、[14]和SwiftAgg+中方案的计算复杂度是基于Reed-Solomon解码复杂度[18]计算的。Reed-Solomon解码复杂度的任何改进都可以应用于这些方案。
与现有方案相比，如表1所示，SwiftAgg+显着降低了服务器通信负载和每个用户的通信负载。同时，与 LightSecAgg 类似，所提出的 SwiftAgg+ 也具有较小的服务器计算复杂度和worst-case的安全保证。
![](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230626195503.png)

### Problem Formulation

#### Notations
H(X)表示随机变量X的熵
I(X;Y)是两个随机变量 X 和 Y 的mutual information

我们考虑联邦学习系统的安全聚合问题，该系统由服务器和 N 个用户 $U_1, ...,U_N$组成。
对于每个$n ∈ [N]$，用户 n 对于某个有限域 F 都有一个大小为 L 的private local model，用 $W_n ∈ \mathbb{F}^L$ 表示。考虑局部模型来自某个联合分布（通常是未知的）：
$$W_1, W_2,...,W_N ∼ P_{W_1,W_2,...,W_N} (W_1, W_2,...,W_N )$$
局部模型的每个entry经过通用线性（仿射）映射后，用一个非负整数表示，都会小于某个 $\ell\in\mathbb{N}$。每个用户 n 也有一个随机变量${\mathcal{Z}}_{n}$的集合，其元素是从 $\mathbb{F}^L$中uniformly选择的 ，并且彼此独立且与本地模型无关。

用户可以使用无差错的专用通信链接相互发送消息，也可以向服务器发送消息。 

$\mathbf{M}_{n\to n^{\prime}}^{(L)}\ \in\ \mathbb{F}^{*}\ \cup\ \{⊥\}$表示用户 n 发送给用户 n′ 的消息。
另外，$\mathbf{X}_{n}^{(L)}\ \in\ \mathbb{F}^{*}\ \cup\ \{⊥\}$表示节点n向服务器发送的消息。空符号⊥表示没有发送消息的情况。

消息$\mathbf{M}_{n\to n^{\prime}}^{(L)}$是关于$W_n$、$Z_n$ 以及节点 n 迄今为止从其他节点接收到的消息的函数。我们用${f}_{n\to n^{\prime}}^{(L)}$表示相应的编码函数。
类似地，消息$\mathbf{X}_{n}^{(L)}$是关于$W_n$、$Z_n$ 以及节点 n 迄今为止从服务器接收到的消息的函数。我们用${g}_{n}^{(L)}$表示相应的编码函数。

对于子集 S ⊆ [N]，我们让 ${\chi_{S}}=\ \{{\bf X}_{n}^{(L)}\}_{n\in S}$表示服务器从集合 S 中的用户那里接收到的消息集。我们假设用户的子集 D ⊂ [N] 退出，即在协议执行期间保持silent（或发送 ⊥ 到其他节点和服务器）。我们将退出用户的数量表示为 D = |D|。

我们还假设身份未知的用户子集 T ⊂ [N] 是半诚实的。意味着T中的用户忠实地遵守协议；然而，他们很好奇，可能会相互串通或与服务器串通以获取有关诚实用户的本地模型的信息。我们假设 |T | ≤ T，对于某些已知的安全参数 T < N − D。

#### 安全聚合方案满足的条件：Correctness和Privacy Constraint
安全聚合方案由编码函数${f}_{n\to n^{\prime}}^{(L)}$和${g}_{n}^{(L)}$ , n, n′ ∈ [N] 组成，满足以下条件：
1. Correctness
   服务器能够使用  $\textstyle X_{[{N}]\backslash{\mathcal{D}}} =\left\{\mathbf{X}_{n}^{\left(L\right)}\right\}_{n\in\left[N]\backslash\\\mathcal{D}\right.}$恢复 $W=\sum_{n\in\left[N]\backslash\\\mathcal{D}\right.}W_n$。更确切地说，
   $$H\bigg(\sum_{n\in[N\,|\backslash\mathcal{D}}^{}{\bf W}_{n}\big|\chi_{[N\,]\backslash\mathcal{D}}\bigg)=0$$
2. Privacy Constraint
   对于任何联合分布$P_{W_1,W_2,...,W_N} (W_1, W_2,...,W_N )$，在收到 $\textstyle X_{[{N}]\backslash{\mathcal{D}}}$并与 T 中的半诚实用户串通后，在他们的aggregation之外，在从它们与半诚实用户的本地模型的相关性推断出的信息之外，服务器不应该获得任何信息关于诚实用户的本地模型。Formally：
   $$I\left({\bf W}_{n},n\in[N]\backslash\mathcal{T};X_{[N]\backslash\mathcal{D}},\bigcup_{k\in\mathcal{T}}\{{\bf M}_{k^{\prime}\to k}^{(L)},k^{\prime}\in[N]\}\bigg|\sum_{n\in[N\,]\,\backslash\,\{\,{\mathcal D}\cup{\mathcal T}\}}\,\mathbf{W}_{n},\,\left\{{\bf W}_{k},\,{\mathcal Z}_{k},\,k\,\in\,{\mathcal T}\,\right\}\right)=0$$

#### user和server的通信负载定义
对于满足上述两个条件的安全聚合方案，我们定义每用户通信负载和服务器通信负载如下：
1. 定义 1（标准化平均per-user通信负载）
   用 $R^{(L)}_{user}$ 表示，定义为用户发送的所有消息的aggregated size，用𝑁𝐿 归一化，即：$$R_{\mathrm{user}}^{(L)}=\frac{1}{N L}\,\sum_{n\in[N],n' \in [N] \backslash n}\ \left({H}(\mathrm{M}_{n\to n^{\prime}}^{(L)})+H(\mathrm{X}_{n}^{(L)})\right)$$
2. 定义 2（标准化服务器通信负载）
   用 $R^{(L)}_{server}$ 表示，定义为服务器接收到的所有消息的aggregated size，用 L 归一化，即：
   $$R_{\mathrm{server}}^{(L)}=\frac{1}{L}\sum_{n\in[N]}H({\bf X}_{n}^{(L)})$$
   
如果存在一系列具有rate tuples $(R^{(L)}_{server}, R^{(L)}_{user})$，L = 1, 2,...的安全聚合方案，我们说pair $(R_{server}, R_{user})$是可实现的。such that：
$$R_{\mathrm{server}}=\operatorname*{lim sup}_{L\to\infty}R_{\mathrm{server}}^{(L)}$$
$$R_{\mathrm{user}}=\operatorname*{lim sup}_{L\to\infty}R_{\mathrm{user}}^{(L)}$$
3. 定义 3（可实现方案的通信图）
   对于安全聚合问题的可实现方案${\mathcal{A}}(N,T,D)$，由 N 个用户和一个服务器组成，我们定义无向通信图${\mathcal{GA}}(\mathcal{V},\mathcal{E_A})$。在此图中， $\mathrm{V~}=~\{U_{1},\ldots\cdot\mathrm{,~}U_{N},{\mathrm{Server}}\}$是代表用户和服务器的顶点集合，$\mathcal{E_A}$是这些顶点之间的活动通信链路对应的边集合。在此图中，如果相应的用户直接相互通信（他们不发送空消息⊥），则两个顶点 v1, v2 ∈ V 之间的边$e ∈ \mathcal{E_A}$存在。

### Main Results
在本节中，我们将介绍通过提出的 SwiftAgg+ 方案实现的per-user和服务器通信负载的主要结果。请注意，操作是在有限域中完成的，该域足够大以避免在聚合过程中触及边界。对于某个素数 p，我们选择一个用 $\mathbb{F}_p$表示的有限域 GF (p)，其中$N(\ell − 1) < p ≤ 2N (\ell − 1)$。

1. 定理 1. 
   考虑一个安全聚合问题，有 N 个用户和一台服务器，其中最多 T 个用户是半诚实的，最多 D 个用户可能会退出。有一个achievable的方案需要：
   $$R_{s e r\nu e r}=\left(1+{\frac{T}{N-T-D}}\right)$$
   $$R_{u s e r}\ \le\left(1\ +\,\frac{T+D}{N+\ T-D}\right)$$为了实现定理 1 中的通信负载，我们提出了 SwiftAgg+，这是联邦学习中一种新颖的安全聚合方案。在 SwiftAgg+ 中，在 T = o(N) 和 D = o(N) 的条件下，每个用户发送的符号数量为 (1 + O( 1/N )) L ，服务器接收到的符号数量为(1 + O( 1/N )) L 以隐私保护的方式计算本地模型的聚合。换句话说，对于较大的N，每个用户的通信负载趋向于$\mathbb{F}_p$中的L个符号，并且服务器的总通信负载也趋向于$\mathbb{F}_p$中的L个符号。
   
2. 定理 2. 
   对于 T = o(N) 和 N − D = O(N)，就所需bits而言，SwiftAgg+ 中的服务器通信负载在within factor 1 of the cut-set lower bound 内。
   
3. 定理 3. 
   对于uniform distributions的局部模型，就所需bits而言，SwiftAgg+ 中的每用户通信负载在within factor $\log_{\ell}{\ell N}$ of the cut-set lower bound，其中 T = o(N) 且 D = o(N) 
   
   Remark 1：
   请注意，T = o(N) 的情况是有充分理由的。由于预算有限，随着用户数量的增长，攻击者攻击固定比例的用户通常会变得异常困难。例如，攻击两个用户中的一个似乎比攻击 100 个用户中的 50 个更容易。由于活动通信链路的数量在联邦学习中很重要，SwiftAgg+还允许我们**减少安全聚合问题中的活动网络连接的数量，但代价是增加通信负载**，使其偏离最佳值。结果由以下定理给出。
   
4. 定理 4. 
   考虑一个安全聚合问题，有 N 个用户和一台服务器，其中最多 T 个用户是半诚实的，最多 D 个用户可能会退出。对于任何 K ∈ N，其中 (T + D + K)|N，存在可实现的方案$\mathcal{A}_{K}\left(N,T,D\right)$，其中有这么多symbols（from $\mathbb{F}_p$）：
   $$R_{s e r\nu e r}^{(\mathcal{A}_{K})}=\;1\,+\,\frac{T}{K}$$$$R_{u s e r}^{(\mathcal{A}_{K})}\ \le\ \left(1\ +\frac{T+D}{K}\right)$$
  该可实现方案 ${\mathcal{G}}_{\mathcal{A}_{K}}\left({\mathcal{V}},{\mathcal{E}}_{\mathcal{A}_{K}}\right)$的通信图由$|{\mathcal{E}}_{\mathcal{A}_{K}}|=\frac{N}{2} (K + T + D + 1)$条边组成。
  
  ✏️Remark2：在定理4中，通过增加参数K，用户通信负载和服务器通信负载都减少了，同时可实现的方案|EAK|中的活动连接数也减少了。增加，反之亦然。这使我们能够在通信负载和通信模式的复杂性（就活动链路的数量而言）之间进行灵活的权衡。
  
  为了实现通信负载和网络连接$|{\mathcal{E}}_{\mathcal{A}_{K}}|$之间的权衡，SwiftAgg+ 将用户划分为一些不相交的组，每个大小为 K + D +T ，其中的用户标号从 1 到 K + D + T。 
  N/(K +D+T) 个组排列成以服务器为根的任意树。模型聚合从树的叶子开始，分三个主要阶段进行： 
  - 第 1 阶段：每个用户将其长度为 L 的本地模型的向量划分为长度为 L/K 的 K 个子向量
  - 第 2 阶段：每个用户使用斜坡共享（ramp sharing） [17] 将其模型的子向量共享给其组内的其他用户
  - 第 3 阶段：每个用户聚合其在第 2 阶段接收到的shares，并将其添加到从其子组中的相应用户接收到的消息中并将结果发送给其父组中相应的用户。这些消息最终到达服务器并用于恢复聚合的本地模型。
    
    ✏️Remark 3：定理 1 中的最小通信负载是通过将 K 设置为 N − D − T 的最大值来实现的。最小通信连接数是通过设置 K = 1 来实现的，这可以简化为[14]中的 SwiftAgg 方案。
    
    ✏️Remark 4：虽然在问题表述中我们让 L → ∞，但所提出的方案适用于 L 的有限值，其中 K |L。如果 K ∤ L，我们可以对局部模型进行zero-pad。


### THE PROPOSED SWIFTAGG+ SCHEME
在本节中，我们正式描述所提出的 SwiftAgg+，它引入了通信负载与用户和服务器之间的活动通信链路数量之间的权衡。考虑一个由一台服务器和 N 个用户 U1, U2, ...，UN组成的网络 ,  其中最多 T 个是半诚实的，可能会相互勾结或与服务器勾结以获取有关其他用户的local models。
此外，最多有D个用户可能会dropout，他们的索引用D表示。

操作需要在有限域内完成，该有限域足够大以避免在聚合过程中触及边界。对于某个素数 p，我们选择一个用 $\mathbb{F}_p$表示的有限域 GF (p)。
每个用户 n 都有一个本地模型$W_n ∈ \mathbb{F}^L$ 和一组随机变量${\mathcal Z}_{n}\;=\;\{{\bf Z}_{n,j},\,j\ \in\ [{T}]\}$，其元素是从$\mathbb{F}^{\frac{L}{K}}_p$中独立且均匀地随机选择的，其中 K ∈ N 且满足(T + D + K)|N。服务器想要恢复幸存用户的aggregated local models，即，$W=\sum_{n\in\left[N]\backslash\\\mathcal{D}\right.}W_n$，而各个模型对半诚实用户和服务器保持private。为了实现这一目标，SwiftAgg+ 采取了以下步骤：

#### Step1：Grouping
N 个用户的集合被任意划分为 Γ 个组，每个组的大小为 $ν \triangleq D + T + K$，用 ${\mathcal{G}}_{1},{\mathcal{G}}_{2},\dots{\mathcal{G}}_{\Gamma}$表示。在每个组中，用户被标记为用户 1 到用户 K + D + T。为了简单起见，我们根据用户 n 在用户组中的位置来引用它。不失一般性，我们令$\gamma\,=\,\lfloor n/\nu\rfloor+1$，并且 t = n mod ν + 1，并将用户 n 放置在组 γ 中的第 t 个位置。或者，我们使用 (γ, t) 来标记用户 n。

#### Step2：Arranging the Groups
这些组排列在任意树上，称为aggregation tree，用 ${\mathcal{T}}\,({\hat{\mathcal{V}}},{\hat{\mathcal{E}}})$表示。聚合树表示聚合的流程。在聚合树中，${\hat{\mathcal{V}}}$是代表组和服务器的一组顶点， ${\hat{V}}=\{{\mathcal{G}}_{1},{\mathcal{G}}_{2},\cdot\cdot\cdot\cdot{\mathcal{G}}_{^{T}},{\mathrm{Server}}\}$和${\hat{\mathcal{E}}}$是表示组之间活动连接的边集。在聚合树中，服务器是根，它只有一个子节点，即最后一组 $\mathcal{G}_{\Gamma}$。例如，对于具有七组用户 $G_1,G_{2},\ldots,G_7$的示例，有五个不同的聚合树。如图3所示。
![](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230630225931.png)

对于位于该树的一个顶点的群$\mathcal{G}_{\gamma}$，令$\mathcal{G}_{\gamma^{+}}$ 代表$\mathcal{G}_{\gamma}$的父群， ${\mathcal{F}}(\gamma,\mathrm{child})$为其子群的索引集。在有根树中，组 γ 的后代是从根开始的路径包含组 γ 的任何组 γ1，并且当且仅当组 γ 是组 γ2 的后代时，组 γ2 是组 γ 的祖先。我们将 ${\mathcal{F}}(\gamma,\mathrm{desc})$定义为 γ 组的后代组的索引集，并且${\mathcal{F}}(\gamma,\mathrm{anc})$作为组 γ 的祖先组的索引集（不包括服务器）。例如，在图3(d)中，$\mathcal{G}_{5^{+}}=\mathcal{G}_{7}$ 是$\mathcal{G}_{5}$和$\mathcal{F}_{5, child}=\{1, 2, 3\}$的父组。另外，G7有set $\mathcal{F}_{7, desc}=\{1, 2, 3, 4, 5, 6\}$，G1 有 set  $\mathcal{F}_{1, anc}=\{5, 7\}$。

#### Step3：Partitioning the Local Models
用户 n 将其本地模型划分为 K 个部分，表示为：
$$\mathbf{W}_{n}=\left[\mathbf{W}_{n,1},\mathbf{W}_{n,2},\ldots,\mathbf{W}_{n,K}\right]$$
是长度为 L/K 的 K 个子向量

#### Step4：Intra-Group Secret Sharing and Aggregation
用户n∈[N]构造下面的多项式：
$$\mathrm{F}_{n}(x)=\sum_{k=1}^{K}\mathrm{W}_{n,k}x^{k-1}+\sum_{j=1}^{T}{\cal Z}_{n,j}x^{K+j-1}$$
这个多项式函数设计会让$x^k$的系数就是local model的第k+1个partition，for k∈(0: k−1)。每个用户n利用多项式$F_n(.)$与其他用户共享其本地模型。

让$\alpha_{t}\in \mathbb{F}_p$, t∈[ν]，是ν个不同的非零常数。
我们将$\alpha_t$分配给所有组的第t个用户，也就是users $(\gamma, t)$，其中$\gamma=1, ..., \Gamma$

在每个组γ中，每个用户$(\gamma, t)$发送其多项式函数在$\alpha_{t'}$处的evaluation，即：$F_{(γ,t)}(α_{t^′})$给用户(γ,t′), t′∈(ν)。如果一个用户(γ,t) drops并保持沉默，$F_{(γ,t)}(α_{t^′})$只是假定为零。

每个用户$(\gamma, t)$计算：
$${\bf Q}_{(\gamma,t)}=\sum_{t^{\prime}\in[v\,]}\,{\bf F}_{(\gamma,t^{\prime})}\,(\alpha_{t})$$
注意,在这个阶段,在每一组中,最多发生ν(ν−1)次通信,每个大小L/K。


#### Step5：Inter-group Communication and Aggregation
在这个阶段, γ组的用户t计算消息（用$S_{(γ,t)}$表示），并将其发送其parent group γ+中的用户t，for 𝛾 ∈ [Γ − 1]。
特别地，如果用户(γ,t)，γ∈(Γ−1]没有任何children groups。即： $\mathcal{F}_{(}\gamma_{\cdot\mathrm{child})}=\emptyset$，那么我们设置：
$$S_{(γ,t)}=Q_{(γ,t)} \tag{8}$$
然后将$S_{(γ,t)}$发送给用户$(\gamma^+,t)$

如果$\mathcal{F}_{(}\gamma_{\cdot\mathrm{child})}≠\emptyset$，用户$(\gamma, t)$会在收到$\{ S_{(γ^-,t)},\gamma^{-}\in F_{(γ,child)}\}$后，将$S_{(γ,t)}$计算为：
$$\mathbf{S}_{(\gamma,t)}=\mathbf{Q}_{(\gamma,t)}+\sum_{\gamma^{-}\in{\mathcal{F}}(\gamma,\mathrm{child})}\mathbf{S}_{(\gamma^{-},t)}$$

如果用户 (γ, t) 没有从$F_{(γ,child)}$中的至少一组接收到$S_{(γ^-,t)}$ ，则它对于协议的其余部分也保持沉默。在此阶段，最多传送 ν(Γ − 1) 条消息，每条消息的大小为 L/K 。图 4 演示了一颗sequential聚合树中的intra-group secret sharing和inter-group communication。
![](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230627000233.png)

#### Step5： Communication with the Server
最后一组的用户 t，即用户 (Г, t) 计算：
$$\mathbf{S}_{(\Gamma,t)}=\mathbf{Q}_{(\Gamma,t)}+\sum_{\gamma^{-}\in{\mathcal{F}}(\gamma,\mathrm{thid})}\mathbf{S}_{(\gamma^{-},t)} \tag{10}$$
for t ∈ [ν]，并将其发送到服务器，

#### Step6：恢复结果
从大小至少为 T + K 的$G_{\Gamma}$ 中的用户子集接收到消息后，服务器可以恢复聚合的本地模型。

✏️Remark 5
在（6）中，我们使用ramp sharing[17]来保持各个本地模型的私有性，但任何其他任意𝑇-private MDS code都可以用于 $F_n(x)$。Ramp sharing使我们能够减少shares的大小，从而在不断缩小的gap内达到cut-set的外部边界（outer-bound）。

✏️Remark 6：
SwiftAgg+ 中组的形成和聚合树的拓扑可能受到网络中实际连接性的限制。

接下来，我们通过证明服务器可以从从组 Γ 接收的消息中恢复$W=\sum_{n\in\left[N]\backslash\\\mathcal{D}\right.}W_n$来证明 SwiftAgg+ 在聚合用户模型方面的正确性。使用递归方程 (8) 至 (10)，$S_{(γ,t)}(\alpha_t)$要么是空消息，要么等于：

$$\begin{array}{c}{{\mathrm{S}_{(\gamma,t)}(\alpha_{t})=\sum_{k=1}^{K}\alpha_{t}{}^{k-1}\sum_{\gamma^{\prime}\in\mathcal{F}_{(\gamma,\mathrm{desc)}}}\sum_{n\in\mathcal{G}_{\gamma^{\prime}}\backslash D}\mathbf{W}_{n,k}}}\\ {{\quad\quad\quad+\sum_{j=1}^{K}\alpha_{t}{}^{K+j-1}\sum_{\gamma^{\prime}\in\mathcal{F}_{(\gamma,\mathrm{desc})}}\sum_{n\in\mathcal{G}_{\gamma^{\prime}}\backslash\mathcal{D}}}} Z_{n,j} \tag{11}\end{array}$$

因此，如果组 Γ 中的用户 t 向服务器发送消息，则它等于$\mathrm{S}_{(\Gamma,t)}(\alpha_{t})$。由(11)式不难看出$\mathrm{S}_{(\Gamma,t)}(\alpha_{t})=F(\alpha_t)$，其中：
$$\mathrm{F}(x)=\sum_{k=1}^{K}x^{k-1}\sum_{n\in[N\backslash D}\mathrm{W}_{n,k}+\sum_{j=1}^{T}x^{K+j-1}\sum_{n\in[N\backslash D}\mathrm{Z}_{n,j} \tag{12}$$
F(x) 是 K + T − 1 次多项式。因此，如果服务器从最后一组接收到至少 T + K 条消息，则可以使用拉格朗日插值来恢复 F(x) 和：
$$\sum_{n\in[N]\setminus D}\mathbf{W}_{n}=\left[\sum_{n\in[N]\setminus\mathbf{D}}\mathbf{W}_{n,1},\sum_{n\in[N]\setminus\mathbf{D}}\mathbf{W}_{n,2},\ldots,\sum_{n\in[N]\setminus\mathbf{D}}\mathbf{W}_{n,K}\right]^{T}$$
回想一下，在 SwiftAgg+ 中，对于 D 中的任何用户$(\gamma, t)$，所有消息$S_{(γ^-,t)},\gamma^{-}\in \{\gamma, F_{(γ,anc)}\}$为空。特别地，对于D中的任何用户(γ，t)，S(Γ，t)(αt)为空。因此最后一组中最多D个用户向服务器发送空消息。由于每个组的大小为 D +T + K，因此服务器对于不同的 αt，至少接收到T + K 个$\mathrm{S}_{(\Gamma,t)}(\alpha_{t})$值 ，从而可以正确地恢复 F(x)。


## Q6 论文中的实验是如何设计的？

### ILLUSTRATIVE EXAMPLES
在本节中，我们提出了所提出的 SwiftAgg+ 方案的两个说明性示例，以在设计参数 K 的不同选择下解决安全聚合问题。这也演示了在 SwiftAgg+ 中通过改变 K 实现的通信负载和通信链路数量之间的权衡。

我们考虑一个由一台服务器和 N = 12 个用户 U1, U2,...，U12组成的联邦学习系统的安全聚合问题。在聚合过程中，最多有 D = 1 个用户可能会退出，最多有 T = 2 个半诚实用户可能会相互串通以获得有关其他用户的本地模型的一些信息。每个用户 n 都有一个本地模型 Wn，它是大小为 L 的向量，

#### A. K = 9 时的最小通信负载
每个用户 n 从$\mathbb{F}^{\frac{L}{9}}$中随机均匀采样两个向量${\mathcal{Z}}_{n}=\{Z_{n,1}, Z_{n,2}\}$，然后执行以下步骤：
1. Partitioning the Local Models
   用户 n 将其本地模型划分为 K = 9 个部分，即：$$\mathrm{W}_{n}=\left[\mathrm{W}_{n,1},\mathrm{W}_{n,2},\ldots,\mathrm{W}_{n,9}\right]^{T}$$每一部分的大小都是L/9
2. 秘密共享和聚合
   用户 n 形成以下多项式：$$\mathbf{F}_{n}(x)=\mathbf{W}_{n.1}+\mathbf{W}_{n.2}x+\mathbf{\cdot\cdot\cdot}+\mathbf{W}_{n.9}x^{8}+\mathbf{Z}_{n.1}x^{9}+\mathbf{Z}_{n.2}x^{10}$$其中前 K = 9 项的系数是用户 n 的局部模型的partitions。
   令 $\alpha_t ∈ \mathbb{F}$, t ∈ [12] 为不同的非零常数。我们将 $\alpha_t$ 分配给用户 t。在此步骤中，每个用户 n 将其在 $\alpha_t$ 处的多项式函数的evaluation，即$\mathbb{F}_n(\alpha_t)$发送给用户 t，for t ∈ [12]。

      ![500](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230628160759.png)
   图1表示用户和服务器之间的连接链路。如图 1 所示，本例中的 G(V, E) 是一个完全图，这意味着所有用户都相互通信以及与服务器通信。如果用户 m 退出并保持沉默，则 $\mathbb{F}_m(\alpha_t)$就被假定为零。
   
   每个用户n计算 $\mathrm{S}_{n}~=~\sum_{n^{\prime}=1}^{12}\,\mathrm{F}_{n^{\prime}}(\alpha_{n})$。在此示例中，假设 U3 退出并且不将其share发送给其他用户。其他用户将其share视为0。在此阶段，最多发生 132 次通信（11x12），每次通信大小为 L/9。
   
3. 与服务器通信
   用户n向服务器发送Sn, n∈[12]。显然在这个例子中,用户3保持沉默和没有发送消息(或空消息⊥)给服务器。
   
4. 恢复结果
   让我们定义：
   $$\mathbf{F}(x){\triangleq}\sum_{n=1}^{12}\mathbf{F}_{n}(x)=\sum_{k=1}^{9}x^{k-1}\sum_{n=1}^{12}\mathbf{W}_{n,k}+x^{9}\sum_{n=1}^{12}\mathbf{Z}_{n,1}+x^{10}\sum_{n=1}^{12}\mathbf{Z}_{n,2}$$

  对于服务器接收到的$n ∈ [12]\backslash \{3\}$ ， Sn，可以验证Sn确实等于$\mathbb{F}(\alpha_1)，\mathbb{F}(\alpha_{2})，\mathbb{F}(\alpha_{4}),..., \mathbb{F}(\alpha_{12})$。
   
   由于F(x)是10次多项式函数，基于拉格朗日插值规则，服务器可以利用未被丢弃的用户的结果来恢复该多项式的所有系数。特别地，服务器可以使用恢复的多项式函数中的$x^k$ 、k ∈ [0 : 8]的系数来恢复$\begin{array}{r}{\sum_{n=1,\\{n \neq 3} }^{12}\mathbf{W}_{n}}\end{array}$。因此，服务器能够恢复幸存用户的本地模型的聚合并且满足正确性约束。


在本例中，每用户通信负载为 4/3L，服务器通信负载为 11/9 L。此外，通信图是一个具有 78 个边和 13 个顶点的完全图，其中由于用户dropout，有12条边上没有发生通信。

#### B. Trading off communication loads for less connections
现在我们考虑一个场景，其中并非所有用户都可以相互通信。 SwiftAgg+ 允许牺牲通信负载以减少所需通信链路的数量。在这种情况下，我们取 K = 3，每个用户从 F L 3 中均匀随机地局部采样两个向量${\mathcal{Z}}_{n}=\{\tilde{Z}_{n,1}, \tilde{Z}_{n,2}\}$。为了减少连接数，每个用户采取以下步骤：
1. Partitioning the Local Models
   用户 n 将其本地模型划分为 K = 9 个部分，即：$$\mathrm{W}_{n}=\left[\mathrm{W}_{n,1},\mathrm{W}_{n,2},\mathrm{W}_{n,3}\right]^{T}$$每一部分的大小都是L/3
2. Grouping
   用户集被任意划分为 Γ = 2 个大小为 ν = K + D + T = 6的组，，用 G1、G2 表示。图 2 表示 这种分区的一个示例，其中 G1 = {U1, U2, U3, U4, U5, U6}，G2 = {U7, U8, U9, U10, U11, U12}。我们还对每个组中的用户进行任意排序。
   为了简化说明，我们可以根据用户n在用户组中的位置来引用用户n。如果用户n是γ组中的第t个用户，我们将其称为用户（γ，t）。例如，在图2中，用户9与用户(2, 3)表达的含义相同。我们交替使用索引 n 或 (γ, t)。
   ![](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230628200130.png)
3. Intra-group秘密共享和聚合
   用户n形成以下多项式：
   $${\bf F}_{n}(x)={\bf W}_{n,1}+{\bf W}_{n,2}x+{\bf W}_{n,3}x^{2}+\tilde{\bf Z}_{n,1}x^{3}+\tilde{\bf Z}_{n,2}x^{4}$$
   令 $α_t \in \mathbb{F}$, $t \in [6]$ 为六个不同的非零常数。我们将 $\alpha_t$ 分配给所有组的用户 t，即用户 (γ, t)，γ = 1, 2。在这一步中，每个用户 (γ, t) 发送其多项式函数在$\alpha_{t'}$处的评估，即将 $F _{(γ,t)} (α_{t′})$，给用户 (γ, t′)，对于 t′ ∈ [6]。
   
   例如，在图2中，用户(2, 1)，实际上是U7：
   发送F7(α1)、F7(α2)、F7(α3)、F7(α4)、F7(α5)、F7(α6) ，
   分别到用户 (2, 1)（或用户 U7，其实是其自身）、用户 (2, 2)（或用户 U8）、用户 (2, 3)（用户 U9）、用户（2, 4）（用户 U10 ）、用户（2, 5）（用户 U11）和用户（2, 6）（用户 U12）。
   如果用户 (γ, t) 退出并保持沉默，则$F _{(γ,t)} (α_{t′})$就被假定为零。
   
   G1 中的第 t 个用户 t ∈ [6] 计算：$$\begin{array}{c}{{{\bf Q}_{(1,t)}={\bf F}_{(1,1)}\left(\alpha_{t}\right)+{\bf F}_{(1,2)}\left(\alpha_{t}\right)+{\bf F}_{(1,3)}\left(\alpha_{t}\right)+{\bf F}_{(1,4)}\left(\alpha_{t}\right)}}\\ {{{}}}\\ {{+{\bf F}_{(1,5)}\left(\alpha_{t}\right)+{\bf F}_{(1,6)}\left(\alpha_{t}\right),}}\end{array}$$
   G2中的第t个用户计算： $$\begin{array}{c}{{{\bf Q}_{(2,t)}={\bf F}_{(2,1)}\left(\alpha_{t}\right)+{\bf F}_{(2,2)}\left(\alpha_{t}\right)+{\bf F}_{(2,3)}\left(\alpha_{t}\right)+{\bf F}_{(2,4)}\left(\alpha_{t}\right)}}\\ {{{}}}\\ {{+{\bf F}_{(2,5)}\left(\alpha_{t}\right)+{\bf F}_{(2,6)}\left(\alpha_{t}\right).}}\end{array}$$
    在此示例中，假设 U3 或用户 (1, 3) 退出并且不将其份额发送给第一组中的其他用户。该组内的其他用户将其份额视为零。在此阶段，每个组内最多发生 30 次通信，每次通信大小为 L/3。
    
4. intra-group通信和聚合
   在这个阶段，用户(1,t)，t∈[6]，计算消息S(1,t) = Q(1,t)，并将其发送给用户(2,t)。用户 (2, t), t ∈ [6] 在收到 S(1,t) 后计算消息 S(2,t) = S(1,t) + Q(2,t) 。
   如果用户 (2, t) 没有收到 S(1,t) ，它也会在协议的其余部分保持沉默。
   在用户 3 退出的这个特定示例中，它没有向用户 9 发送消息，因此用户 9 也保持沉默。
   
5. 与服务器通信
   最后一组的用户t，即用户(2,t)发送S(2,t)到服务器，t∈[6]。显然，在此示例中，用户 9 保持沉默并且不向服务器发送任何内容（或空消息 ⊥）。
   
6. 恢复结果
   让我们定义：
   ![500](https://cdn.jsdelivr.net/gh/LonelyMoonDesert/BlogImgBed2@main/img/20230628233332.png)
   可以验证服务器接收到的 S(2,t) ，对于 t = 1, 2, 4, 5, 6 确实等于 F(αt)，对于 t = 1, 2, 4, 5, 6
   由于F(x)是4次多项式函数，基于拉格朗日插值规则，服务器可以使用5个未丢弃的用户的结果来恢复该多项式的所有系数。因此，服务器能够恢复幸存用户的本地模型的聚合，即$\begin{array}{r}{\sum_{n=1,\\{n \neq 3} }^{12}\mathbf{W}_{n}}\end{array}$并且满足正确性约束。
   
在此示例中，每用户通信负载为 2L，服务器通信负载为 5/3 L。此外，通信图具有 42 条边和 13 个顶点，其中由于用户丢失，7 条边上没有发生通信。与Example 1相比，通信负载增加，而用户之间的连接数减少。通过选择 ν = T + D + 1 = 4 并具有三个组（where no partitioning of local models is performed），可以最小化连接数量。
## Q7 用于定量评估的数据集和baselines是什么？

## Q8 论文中的实验及结果有没有很好地支持需要验证的科学假设？

## Q9 这篇论文到底有什么贡献？
在本文中，我们提出了 SwiftAgg+，一种用于联邦学习中模型聚合的安全聚合协议，它实现了通信负载和网络连接之间的权衡。通过对用户进行分组，精心设计组内和组间的秘密共享和聚合方法，SwiftAgg+能够在最多D个退出用户的情况下实现正确聚合，并提供最坏情况下的安全保证，防止最多T个用户串通一个好奇的服务器。此外，SwiftAgg+可以通过选择不同深度的聚合树来灵活地控制每次训练迭代的延迟。与之前的安全聚合协议相比，SwiftAgg+显着降低了通信负载。对于 T = o(N ) 和 N − D = O(N )，就所需位数而言，SwiftAgg+ 中的服务器通信负载在割集下限的因子 1 内。此外，在均匀分布的本地模型的情况下，只要 T = o(N ) 且 D = o(N )，SwiftAgg+ 中的每用户通信负载就在割集下界的 logl lN 因子之内。
## Q10 下一步呢？有什么工作可以继续深入？

### Ideas
- 不知为何，感觉这篇文章有点点伪需求？因为之前的安全聚合并不需要用户之间两两有连接，table1的对比其实也看不出相对于其他方法的优势所在
- 但是我们可以根据表格来思考一下，什么情况下，用什么方案会使得通信率较低

## New Concepts


