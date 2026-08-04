---
layout: single
title: "Before the Boom"
date: 2026-08-03
topic: "AI History"
summary: "From symbolic AI, backpropagation, and the foundations of deep learning to neural language models, LSTMs, sequence-to-sequence learning, and attention: the technical lineage that led to the Transformer."
permalink: /blog/before-the-boom/
author_profile: true
read_time: true
comments: false
share: false
related: false
---

<div id="before-boom-preview">
  <style>
    #before-boom-preview {
      color-scheme: light dark;
      width: 100%;
      max-width: 1180px;
      margin: 32px auto 64px;
      padding: 0 20px;
      color: light-dark(#24292f, #e8e9eb);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }
    #before-boom-preview * { box-sizing: border-box; }
    #before-boom-preview .site-window {
      overflow: hidden;
      border: 1px solid light-dark(#d8dce1, #3a3d43);
      border-radius: 14px;
      background: light-dark(#ffffff, #202124);
      box-shadow: 0 16px 42px light-dark(rgba(26,31,36,.10), rgba(0,0,0,.32));
    }
    #before-boom-preview .site-nav {
      display: flex;
      align-items: center;
      gap: 24px;
      padding: 18px 28px;
      border-bottom: 1px solid light-dark(#eceef1, #34363b);
      background: light-dark(#ffffff, #242529);
    }
    #before-boom-preview .site-name {
      margin-right: auto;
      font-weight: 500;
      letter-spacing: -.01em;
    }
    #before-boom-preview .site-nav a {
      color: light-dark(#5a6068, #b8bbc1);
      font-size: .88rem;
      text-decoration: none;
    }
    #before-boom-preview .site-nav a:hover,
    #before-boom-preview .site-nav a:focus-visible {
      color: light-dark(#111418, #ffffff);
    }
    #before-boom-preview .site-nav a.active {
      color: light-dark(#111418, #ffffff);
      font-weight: 500;
    }
    #before-boom-preview .site-body {
      display: grid;
      grid-template-columns: 190px minmax(0, 1fr);
      gap: 44px;
      padding: 42px 44px 56px;
    }
    #before-boom-preview .author {
      align-self: start;
      position: sticky;
      top: 28px;
      color: light-dark(#555b63, #b9bcc2);
      font-size: .82rem;
    }
    #before-boom-preview .author-mark {
      display: grid;
      width: 72px;
      height: 72px;
      margin-bottom: 16px;
      place-items: center;
      border-radius: 50%;
      background: light-dark(#e9edf2, #35383e);
      color: light-dark(#69717b, #c9ccd2);
      font-size: 1.2rem;
      font-weight: 500;
    }
    #before-boom-preview .author strong {
      display: block;
      margin-bottom: 7px;
      color: light-dark(#202429, #f0f1f2);
      font-size: .96rem;
      font-weight: 500;
    }
    #before-boom-preview .author p {
      margin: 0;
      line-height: 1.55;
    }
    #before-boom-preview .author-meta {
      margin-top: 22px;
      padding-top: 18px;
      border-top: 1px solid light-dark(#e4e7eb, #393c42);
      line-height: 1.7;
    }
    #before-boom-preview .article {
      min-width: 0;
      max-width: 720px;
    }
    #before-boom-preview .article-tag {
      margin: 0 0 12px;
      color: light-dark(#767d86, #a8abb1);
      font-size: .72rem;
      font-weight: 500;
      letter-spacing: .13em;
      text-transform: uppercase;
    }
    #before-boom-preview .article h1 {
      margin: 0;
      color: light-dark(#14171a, #f8f8f9);
      font-family: Georgia, "Times New Roman", serif;
      font-size: clamp(2.25rem, 6vw, 4.25rem);
      font-weight: 400;
      letter-spacing: -.045em;
      line-height: .98;
    }
    #before-boom-preview .article-subtitle {
      margin: 14px 0 18px;
      color: light-dark(#555c65, #bdc0c5);
      font-family: Georgia, "Times New Roman", serif;
      font-size: clamp(1.08rem, 2vw, 1.35rem);
      line-height: 1.5;
    }
    #before-boom-preview .article-deck {
      display: flex;
      flex-wrap: wrap;
      gap: 8px 16px;
      margin: 0 0 36px;
      padding: 15px 0 17px;
      border-top: 1px solid light-dark(#e4e7eb, #393c42);
      border-bottom: 1px solid light-dark(#e4e7eb, #393c42);
      color: light-dark(#6a717a, #aeb2b8);
      font-size: .78rem;
      letter-spacing: .02em;
    }
    #before-boom-preview .article p,
    #before-boom-preview .article li {
      color: light-dark(#33383e, #d4d6da);
      font-family: Georgia, "Times New Roman", "Noto Serif SC", serif;
      font-size: 1.02rem;
      line-height: 1.82;
    }
    #before-boom-preview .article p {
      margin: 0 0 1.2em;
    }
    #before-boom-preview .article h2 {
      margin: 2.6em 0 .75em;
      padding-top: .35em;
      color: light-dark(#171a1e, #f2f3f4);
      font-family: Georgia, "Times New Roman", "Noto Serif SC", serif;
      font-size: clamp(1.55rem, 3vw, 2.05rem);
      font-weight: 500;
      letter-spacing: -.025em;
      line-height: 1.25;
    }
    #before-boom-preview .article h3 {
      margin: 2em 0 .65em;
      color: light-dark(#202429, #ebedef);
      font-family: Georgia, "Times New Roman", "Noto Serif SC", serif;
      font-size: 1.18rem;
      font-weight: 600;
      line-height: 1.4;
    }
    #before-boom-preview .article a {
      color: light-dark(#315c87, #9bc3ec);
      text-decoration-color: light-dark(#a8bfd5, #587a9b);
      text-underline-offset: .16em;
    }
    #before-boom-preview .article blockquote {
      margin: 2em 0;
      padding: 1.1em 1.35em;
      border-left: 3px solid light-dark(#496f96, #8bb6df);
      background: light-dark(#f5f8fb, #282d33);
      color: light-dark(#293039, #e2e5e8);
    }
    #before-boom-preview .article blockquote p {
      margin: 0;
      color: inherit;
      font-size: 1.08rem;
    }
    #before-boom-preview .equation-note {
      overflow-x: auto;
      margin: 1.55em 0 1.8em;
      padding: 18px 20px;
      border: 1px solid light-dark(#dde3e9, #3c424a);
      border-radius: 10px;
      background: light-dark(#fafbfd, #25282d);
    }
    #before-boom-preview .equation-note p:last-child { margin-bottom: 0; }
    #before-boom-preview .equation-label {
      display: block;
      margin-bottom: 9px;
      color: light-dark(#6a737d, #adb2b9);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      font-size: .7rem;
      font-weight: 600;
      letter-spacing: .11em;
      text-transform: uppercase;
    }
    #before-boom-preview .article table {
      width: 100%;
      margin: 1.5em 0 2em;
      border-collapse: collapse;
      font-size: .85rem;
    }
    #before-boom-preview .article th,
    #before-boom-preview .article td {
      padding: 11px 10px;
      border-bottom: 1px solid light-dark(#e1e5e9, #3b3f45);
      text-align: left;
      vertical-align: top;
    }
    #before-boom-preview .article th {
      color: light-dark(#343a40, #e1e3e6);
      font-size: .73rem;
      font-weight: 600;
      letter-spacing: .06em;
      text-transform: uppercase;
    }
    #before-boom-preview .article td {
      color: light-dark(#4c535b, #c7cacf);
      line-height: 1.55;
    }
    #before-boom-preview .article code {
      border-radius: 4px;
      background: light-dark(#eef1f4, #30343a);
      color: light-dark(#25384b, #d7e8f7);
      font-size: .86em;
    }
    #before-boom-preview .era-marker {
      display: inline-block;
      margin-bottom: .55em;
      color: light-dark(#6d7680, #aeb3ba);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      font-size: .72rem;
      font-weight: 600;
      letter-spacing: .12em;
      text-transform: uppercase;
    }
    #before-boom-preview .synthesis {
      margin: 2.4em 0;
      padding: 22px 24px;
      border: 1px solid light-dark(#ccd9e5, #45576a);
      border-radius: 12px;
      background: light-dark(#f4f8fc, #252c33);
    }
    #before-boom-preview .synthesis h3 { margin-top: 0; }
    #before-boom-preview .synthesis p:last-child { margin-bottom: 0; }
    #before-boom-preview .references {
      margin-top: 3em;
      padding-top: 1.4em;
      border-top: 1px solid light-dark(#dfe3e7, #3c3f45);
    }
    #before-boom-preview .references ol { padding-left: 1.25em; }
    #before-boom-preview .references li {
      margin-bottom: .72em;
      font-size: .88rem;
      line-height: 1.55;
    }
    @media (max-width: 820px) {
      #before-boom-preview { margin-top: 20px; padding: 0 12px; }
      #before-boom-preview .site-nav { gap: 15px; padding: 16px 20px; }
      #before-boom-preview .site-nav a:not(.active) { display: none; }
      #before-boom-preview .site-body {
        grid-template-columns: 1fr;
        gap: 30px;
        padding: 34px 26px 44px;
      }
      #before-boom-preview .author {
        position: static;
        display: grid;
        grid-template-columns: 58px minmax(0, 1fr);
        column-gap: 14px;
        align-items: center;
      }
      #before-boom-preview .author-mark {
        width: 58px;
        height: 58px;
        margin: 0;
      }
      #before-boom-preview .author-meta {
        grid-column: 1 / -1;
        margin-top: 15px;
        padding-top: 14px;
      }
    }
    @media (max-width: 520px) {
      #before-boom-preview .site-window { border-radius: 10px; }
      #before-boom-preview .site-body { padding: 28px 20px 38px; }
      #before-boom-preview .article h1 { font-size: 2.55rem; }
      #before-boom-preview .article p,
      #before-boom-preview .article li { font-size: .98rem; line-height: 1.75; }
      #before-boom-preview .article table { display: block; overflow-x: auto; white-space: nowrap; }
      #before-boom-preview .equation-note { padding: 15px 14px; }
    }
    /* Use the site's native blog layout; this wrapper only scopes optional article styles. */
    #before-boom-preview {
      display: contents;
      color-scheme: normal;
      color: inherit;
      font-family: inherit;
    }
    #before-boom-preview mjx-container[display="true"],
    #before-boom-preview table {
      display: block;
      max-width: 100%;
      overflow-x: auto;
      overflow-y: hidden;
    }
  </style>

  <div markdown="1">
*Technical History · Part I*

*A theoretical and technical prehistory of modern language models, from symbolic reasoning, backpropagation, and representation learning to recurrent networks, sequence modeling, and attention.*

Modern language models are often described as the product of the Transformer architecture combined with computation at scale. This account is not wrong, but it can obscure a more important fact: the architectural breakthrough of 2017 did not appear in isolation. It depended on a collection of theoretical objects and engineering components developed over several decades, including differentiable computation, backpropagation, distributed representations, probabilistic language modeling, stable optimization, recurrent states, gated memory, encoder–decoder architectures, and content-addressed attention.

This article traces the technical lineage that preceded the Transformer. Its purpose is not merely to list milestones. Instead, it asks three questions of each stage: What difficulty was it designed to solve? What mathematical structure did it introduce? Why did that structure become an essential part of later language models?

> The history of the Transformer should not begin with self-attention. It should begin with the problem of expressing intelligence as an optimizable computation graph.

## 1. Two Traditions of Artificial Intelligence: Rules and Learning

<span class="era-marker">1940s–1980s · Symbolic systems and early learning</span>

Early artificial intelligence developed primarily along two lines. Symbolic AI represented knowledge through symbols, propositions, and rules, and then derived conclusions through search and logical inference. Connectionism instead sought to make systems adjust the strengths of their connections from data, allowing internal representations to emerge from experience.

In a symbolic system, a typical problem can be written as state-space search. Let \\(\mathcal{S}\\) denote the set of states, \\(\mathcal{A}(s)\\) the actions available in state \\(s\\), and \\(T(s,a)\\) the transition function. The objective is to find a path from an initial state \\(s_0\\) to a goal set \\(\mathcal{G}\\). With an additional utility function, rational decision-making can be expressed as

<div class="equation-note">
<span class="equation-label">Expected-utility decision</span>

$$
a^{*}=\arg\max_{a\in\mathcal{A}(s)}
\mathbb{E}\!\left[U(s')\mid s,a\right].
$$

This formulation establishes the basic language of states, actions, and consequences. Contemporary planning agents still rely on closely related abstractions. The main difference is that state representation, action selection, and value estimation are now increasingly performed by learned systems.
</div>

Expert systems encoded knowledge as large collections of if–then rules. Given a knowledge base \\(K\\) and a query \\(q\\), an inference engine attempted to determine whether \\(K\models q\\). This approach succeeded in domains with clear boundaries and stable rules, but it also revealed three persistent problems: knowledge acquisition was expensive, manually written rules could not cover open environments, and the resulting systems were brittle under distribution shifts and exceptions. Several downturns in AI during the 1970s and 1980s arose partly from the gap between promised capabilities and actual scalability.

Learning-based methods adopted a different position. Rather than requiring humans to specify every rule, they searched for parameters \\(\theta\\) that minimized empirical risk on a dataset \\(\{(x_i,y_i)\}_{i=1}^{N}\\):

<div class="equation-note">
<span class="equation-label">Empirical risk minimization</span>

$$
\theta^{*}=\arg\min_{\theta}
\frac{1}{N}\sum_{i=1}^{N}\ell\!\left(f_{\theta}(x_i),y_i\right).
$$

Most modern deep-learning procedures can be understood as different parameterizations, loss designs, and numerical solutions to this objective.
</div>

## 2. From Artificial Neurons to the Perceptron

[McCulloch and Pitts (1943)](https://doi.org/10.1007/BF02478259) abstracted a neuron as a weighted computational unit with a threshold. Given inputs \\(x_1,\ldots,x_d\\), its output is

$$
y=\mathbf{1}\!\left[\sum_{i=1}^{d}w_i x_i+b\ge 0\right].
$$

The importance of this model does not lie in its biological realism. It supplied a composable computational primitive: a linear transformation followed by a nonlinear function. Fully connected layers, convolutional layers, and the projection matrices used in attention all inherit this basic structure.

[Rosenblatt's perceptron (1958)](https://doi.org/10.1037/h0042519) added a data-driven rule for updating the weights. For binary classification, one common form is

$$
\hat y_t=\mathbf{1}[w_t^{\top}x_t+b_t\ge 0],
\qquad
w_{t+1}=w_t+\eta(y_t-\hat y_t)x_t.
$$

When the data are linearly separable, the perceptron update converges to a separating hyperplane. A single-layer linear classifier, however, cannot represent nonlinear relations such as XOR. This limitation showed that genuinely complex representations require multiple composed layers. That requirement immediately raised another question: how should each layer know how to modify its own parameters?

## 3. Multilayer Networks and Backpropagation

A multilayer perceptron composes simple transformations layer by layer. Let \\(h^{(0)}=x\\). The \\(\ell\\)-th layer is

$$
h^{(\ell)}=\phi\!\left(W^{(\ell)}h^{(\ell-1)}+b^{(\ell)}\right),
\qquad \ell=1,\ldots,L.
$$

Depth allows a model to construct hierarchical representations, but it also creates complex dependencies among parameters. [Rumelhart, Hinton, and Williams (1986)](https://doi.org/10.1038/323533a0) popularized the use of backpropagation to learn internal representations. Its mathematical basis is the chain rule. If the loss is \\(\mathcal{L}\\), adjacent layers satisfy

<div class="equation-note">
<span class="equation-label">Backpropagation</span>

$$
\frac{\partial \mathcal{L}}{\partial h^{(\ell-1)}}
=
\frac{\partial \mathcal{L}}{\partial h^{(\ell)}}
\frac{\partial h^{(\ell)}}{\partial h^{(\ell-1)}}.
$$

The error at the output can therefore be propagated backward through the computation graph to every parameter. Gradient descent then performs the update

$$
\theta_{t+1}=\theta_t-\eta_t\nabla_{\theta}\mathcal{L}(\theta_t).
$$
</div>

Backpropagation is not a particular network architecture. It is a mechanism for credit assignment: it determines which intermediate computations are responsible for a prediction error and how much each parameter should change. Modern automatic-differentiation systems perform the same operation, while organizing local derivatives over complex computation graphs into efficient programs.

## 4. Why Deep Networks Are Difficult to Train

If a network or recurrent system spans \\(T\\) computational steps, its gradient typically contains a product of Jacobian matrices:

$$
\frac{\partial h_T}{\partial h_t}
=
\prod_{k=t+1}^{T}
\frac{\partial h_k}{\partial h_{k-1}}.
$$

When the dominant singular values of these matrices remain below one, the gradient approaches zero; when they remain above one, it grows rapidly. These are the vanishing- and exploding-gradient problems. The former prevents early layers and distant states from learning effectively, while the latter makes optimization numerically unstable.

### Gradient clipping as a constrained update

After backpropagation, collect all parameter gradients into one vector

$$
g=\nabla_{\theta}\mathcal{L},
\qquad
\|g\|_2=\sqrt{\sum_i g_i^2}.
$$

Global norm clipping constrains the update to an \\(L_2\\) ball of radius \\(\tau\\). It can be written as the Euclidean projection

$$
g_{\mathrm{clip}}
=
\operatorname*{arg\,min}_{\tilde g}
\frac{1}{2}\|\tilde g-g\|_2^2
\quad
\text{subject to}
\quad
\|\tilde g\|_2\leq\tau.
$$

If \\(g\\) already lies inside the ball, the projection leaves it unchanged. Otherwise, the nearest feasible point lies on the same ray as \\(g\\), but has norm \\(\tau\\):

<div class="equation-note">
<span class="equation-label">Global L2 gradient clipping</span>

$$
g_{\mathrm{clip}}
=
\begin{cases}
g, & \|g\|_2\leq\tau,\\[4pt]
\displaystyle \tau\frac{g}{\|g\|_2}, & \|g\|_2>\tau.
\end{cases}
$$

The second branch preserves the gradient direction while replacing its magnitude by the clipping threshold. Clipping therefore limits a single unstable update; it does not repair the underlying source of exploding gradients.
</div>

In PyTorch, clipping is applied after gradients have been computed and before the optimizer updates the parameters:

```python
optimizer.zero_grad()
loss.backward()

total_norm = torch.nn.utils.clip_grad_norm_(
    model.parameters(),
    max_norm=1.0,
)

optimizer.step()
```

Here, `total_norm` is the total gradient norm before clipping, so it can also be logged as a diagnostic signal.

### Measuring gradient gain across layers

The same Jacobian view gives a more local description of vanishing gradients. Let

$$
\delta_k=\frac{\partial\mathcal{L}}{\partial h_k},
\qquad
J_k=\frac{\partial h_{k+1}}{\partial h_k}.
$$

Backpropagation through one layer gives

$$
\delta_k=J_k^{\top}\delta_{k+1}.
$$

Define the gradient gain at layer \\(k\\) as

$$
\gamma_k
=
\frac{\|\delta_k\|_2}{\|\delta_{k+1}\|_2}
=
\frac{\|J_k^{\top}\delta_{k+1}\|_2}
{\|\delta_{k+1}\|_2}.
$$

Across \\(K\\) layers, these local gains multiply:

$$
\frac{\|\delta_0\|_2}{\|\delta_K\|_2}
=
\prod_{k=0}^{K-1}\gamma_k,
\qquad
\log\frac{\|\delta_0\|_2}{\|\delta_K\|_2}
=
\sum_{k=0}^{K-1}\log\gamma_k.
$$

Persistent values \\(\gamma_k<1\\) produce exponential attenuation, while persistent values \\(\gamma_k>1\\) produce exponential amplification. This also explains why an isolated small gradient is not sufficient evidence of vanishing gradients: the relevant signal is the systematic reduction of gradient norm across depth or time.

As an illustrative regularizer, one could penalize deviations of the local gain from one:

$$
\Omega
=
\frac{1}{K}\sum_{k=0}^{K-1}(\gamma_k-1)^2,
\qquad
\mathcal{L}_{\mathrm{total}}
=
\mathcal{L}_{\mathrm{task}}+\lambda\Omega.
$$

This objective encourages norm preservation, but it should be interpreted as a diagnostic construction rather than a standard remedy. Computing it exactly may require higher-order differentiation, and forcing every layer to preserve gradient norm can interfere with useful task-specific dynamics. Initialization, gating, normalization, and residual paths usually address the same problem more directly.

A collection of training components developed after 2010 gradually transformed models that were merely expressive in theory into systems that could be optimized in practice.

| Component | Representative work | Mathematical or engineering role |
|---|---|---|
| Xavier initialization | Glorot & Bengio, 2010 | Sets the weight variance to approximately \\(2/(n_{in}+n_{out})\\), preserving the scale of forward signals and backward gradients |
| ReLU | Glorot et al., 2011 | Uses \\(\max(0,x)\\) to reduce the saturation associated with sigmoid activations |
| Gradient clipping | Pascanu et al., 2013 | Replaces \\(g\\) with \\(c g/\|g\|\\) when \\(\|g\|>c\\), limiting exploding gradients |
| Dropout | Srivastava et al., 2014 | Randomly masks units during training, reducing fragile co-adaptation among features |
| Adam | Kingma & Ba, 2014 | Estimates the first and second moments of gradients to provide parameter-wise adaptive step sizes |
| BatchNorm | Ioffe & Szegedy, 2015 | Normalizes activations using batch statistics, improving the optimization of deep vision networks |
| Residual connection | He et al., 2016 | Learns \\(y=x+F(x)\\), providing short paths for signals and gradients |
| LayerNorm | Ba et al., 2016 | Normalizes across the feature dimension of each example, making it more suitable for sequence models |

### Two routes from SGD to Adam

Adam is easiest to understand not as an isolated algorithm, but as the point where two lines of optimizer research meet. Both begin with stochastic gradient descent:

$$
g_t=\nabla_{\theta}\mathcal{L}_t(\theta_{t-1}),
\qquad
\theta_t=\theta_{t-1}-\eta g_t.
$$

The two lines address different weaknesses of this update:

1. **Adaptive-step route:** How should each parameter receive a learning rate appropriate to its own gradient scale? A useful conceptual lineage is Rprop → AdaGrad → RMSProp.
2. **Momentum route:** How should updates accumulate consistent directions while suppressing noisy oscillation? This leads from classical momentum to Nesterov-style look-ahead and exponential first-moment estimation.

These are conceptual rather than strict genealogical arrows. AdaGrad is not algebraically derived from Rprop, for example, but both replace one global step rule with parameter-wise adaptation.

#### Route I: adaptive learning rates

**Rprop: adjust each step from sign consistency.** A single learning rate \\(\eta\\) treats all coordinates equally even when their gradient scales differ substantially. Rprop takes an early coordinate-wise approach. It discards gradient magnitude and uses only the sign of each coordinate:

$$
\theta_{t,i}
=
\theta_{t-1,i}
-
\operatorname{sign}(g_{t,i})\Delta_{t,i}.
$$

The step size grows when consecutive gradients agree in sign and shrinks when they disagree:

$$
\Delta_{t,i}
=
\begin{cases}
\min(\eta_{+}\Delta_{t-1,i},\Delta_{\max}),
& g_{t,i}g_{t-1,i}>0,\\[4pt]
\max(\eta_{-}\Delta_{t-1,i},\Delta_{\min}),
& g_{t,i}g_{t-1,i}<0,\\[4pt]
\Delta_{t-1,i},
& g_{t,i}g_{t-1,i}=0,
\end{cases}
$$

where \\(\eta_{+}>1\\) and \\(0<\eta_{-}<1\\). Repeated agreement suggests that movement along that coordinate is stable; a sign reversal suggests that the previous step may have crossed a local optimum.

**AdaGrad: normalize by cumulative squared gradients.** AdaGrad uses gradient magnitude to construct a separate effective learning rate for each coordinate. With all products and square roots interpreted elementwise,

$$
G_t
=
G_{t-1}+g_t\odot g_t
=
\sum_{j=1}^{t}g_j\odot g_j,
$$

$$
\theta_t
=
\theta_{t-1}
-
\eta\frac{g_t}{\sqrt{G_t}+\epsilon}.
$$

Coordinates with consistently large gradients acquire a larger denominator and therefore a smaller effective step. However, because \\(G_t\\) only increases, AdaGrad's effective learning rates can eventually become extremely small.

**RMSProp: replace the full history with a moving second moment.** RMSProp replaces the unbounded cumulative sum with an exponential moving average:

$$
v_t
=
\rho v_{t-1}
+
(1-\rho)g_t\odot g_t,
$$

$$
\theta_t
=
\theta_{t-1}
-
\eta\frac{g_t}{\sqrt{v_t}+\epsilon}.
$$

The common principle behind these methods can be derived by asking that the root-mean-square update of coordinate \\(i\\) remain near a target scale \\(\eta\\):

$$
\sqrt{\mathbb{E}\!\left[(\Delta\theta_i)^2\right]}
\approx \eta.
$$

If \\(\Delta\theta_i=-\alpha_i g_i\\), then

$$
\sqrt{\mathbb{E}\!\left[\alpha_i^2g_i^2\right]}
\approx\eta
\quad\Longrightarrow\quad
\alpha_i
\approx
\frac{\eta}{\sqrt{\mathbb{E}[g_i^2]}}.
$$

The algorithms on this route differ largely in how they estimate the second moment \\(\mathbb{E}[g_i^2]\\): AdaGrad uses a cumulative history, while RMSProp uses an exponential moving average that can forget obsolete gradient scales.

#### Route II: momentum and direction smoothing

The adaptive-step route controls **how far** to move along each coordinate. Momentum addresses a different question: **which direction remains reliable across multiple noisy minibatches?** In a form aligned with Adam's notation,

$$
m_t
=
\beta m_{t-1}
+
(1-\beta)g_t,
\qquad
\theta_t
=
\theta_{t-1}-\eta m_t.
$$

Unrolling the recurrence shows that momentum is an exponentially weighted average of past gradients:

$$
m_t
=
(1-\beta)
\sum_{i=1}^{t}\beta^{t-i}g_i.
$$

Gradients that repeatedly point in the same direction accumulate, while rapidly alternating components partially cancel. Momentum therefore acts as a low-pass filter: it accelerates movement along stable directions and reduces oscillation along high-curvature directions.

Classical momentum is often written as \\(u_t=\mu u_{t-1}+g_t\\), followed by \\(\theta_t=\theta_{t-1}-\eta u_t\\). This differs from the normalized exponential-average form only by a constant rescaling that can be absorbed into the learning rate.

Nesterov momentum refines the same route by evaluating the gradient near a look-ahead position:

$$
g_t
=
\nabla_{\theta}
\mathcal{L}_t
\!\left(
\theta_{t-1}-\eta\beta m_{t-1}
\right).
$$

The look-ahead gradient can correct the trajectory before the full momentum step is taken. Vanilla Adam does not directly contain the complete Nesterov update, but it inherits the broader idea of stabilizing direction through an exponential first-moment estimate.

#### Adam: the merger of the two routes

Conceptually, Adam combines

$$
\underbrace{\text{momentum-like first moment}}_{\text{direction}}
\quad+\quad
\underbrace{\text{RMSProp-like second moment}}_{\text{coordinate scale}}
\quad+\quad
\underbrace{\text{bias correction}}_{\text{zero initialization}}
\quad\Longrightarrow\quad
\text{Adam}.
$$

Its update can be written as

$$
m_t=\beta_1m_{t-1}+(1-\beta_1)g_t,
\qquad
v_t=\beta_2v_{t-1}+(1-\beta_2)g_t^2,
$$

$$
\hat m_t=\frac{m_t}{1-\beta_1^t},
\qquad
\hat v_t=\frac{v_t}{1-\beta_2^t},
\qquad
\theta_{t+1}=\theta_t-\eta\frac{\hat m_t}{\sqrt{\hat v_t}+\epsilon}.
$$

The correction factors arise because both moving averages are initialized at zero. Assume for the moment that gradients have a stationary mean \\(\mathbb{E}[g_t]=\mu\\) and that \\(m_0=0\\). Expanding the recurrence gives

$$
m_t
=
(1-\beta_1)
\sum_{i=1}^{t}\beta_1^{t-i}g_i.
$$

Taking expectations and evaluating the geometric series,

$$
\begin{aligned}
\mathbb{E}[m_t]
&=(1-\beta_1)
\sum_{i=1}^{t}\beta_1^{t-i}\mu\\
&=(1-\beta_1)\mu
\sum_{k=0}^{t-1}\beta_1^k\\
&=(1-\beta_1)\mu
\frac{1-\beta_1^t}{1-\beta_1}\\
&=(1-\beta_1^t)\mu.
\end{aligned}
$$

Thus \\(m_t\\) systematically underestimates the first moment early in training. Dividing by \\(1-\beta_1^t\\) removes this initialization bias:

$$
\hat m_t=\frac{m_t}{1-\beta_1^t}.
$$

The same argument applied to \\(v_t\\), under the stationary approximation \\(\mathbb{E}[g_t^2]=\nu\\), yields

$$
\mathbb{E}[v_t]=(1-\beta_2^t)\nu,
\qquad
\hat v_t=\frac{v_t}{1-\beta_2^t}.
$$

Bias correction matters most during the first updates, when \\(\beta_1^t\\) and \\(\beta_2^t\\) are not yet negligible. Adam therefore combines a direction-smoothed first moment with a scale-normalizing second moment while correcting the transient bias introduced by zero initialization.

### Knowledge distillation: why temperature is squared

Not every important pre-Transformer development was aimed at making networks deeper. [Knowledge distillation (Hinton, Vinyals, and Dean, 2015)](https://arxiv.org/abs/1503.02531) addressed a different problem: how to transfer the behavior of a large teacher or ensemble into a smaller student. Its central claim is that knowledge is present not only in the correct label, but also in the teacher's relative preferences among incorrect classes.

Let \\(v_i\\) denote the teacher logit for class \\(i\\), \\(z_i\\) the corresponding student logit, and \\(T>0\\) the temperature. Their softened distributions are

$$
p_i^{(T)}
=
\frac{\exp(v_i/T)}
{\sum_j\exp(v_j/T)},
\qquad
q_i^{(T)}
=
\frac{\exp(z_i/T)}
{\sum_j\exp(z_j/T)}.
$$

At \\(T=1\\), these are ordinary softmax probabilities. Increasing \\(T\\) produces a higher-entropy distribution, making small differences among non-target classes easier to observe. Those relative probabilities convey what is often called the teacher's *dark knowledge*: for example, that an image classified as a BMW is more similar to another car than to a carrot, even when both alternatives receive low probability.

The student is commonly trained with both a soft-target loss and the ordinary hard-label loss:

$$
\mathcal{L}_{\mathrm{soft}}
=
-\sum_i
p_i^{(T)}
\log q_i^{(T)},
\qquad
\mathcal{L}_{\mathrm{hard}}
=
-\sum_i y_i\log q_i^{(1)}.
$$

A standard combined objective is

<div class="equation-note">
<span class="equation-label">Distillation objective</span>

$$
\mathcal{L}
=
\lambda T^2\mathcal{L}_{\mathrm{soft}}
+
(1-\lambda)\mathcal{L}_{\mathrm{hard}}.
$$

The factor T² does not change which student distribution minimizes the soft loss. It compensates for the way temperature reduces the magnitude of its gradients, keeping the soft and hard objectives on comparable scales as the temperature changes.
</div>

To see this, first differentiate the log-softmax:

$$
\frac{\partial\log q_j^{(T)}}{\partial z_i}
=
\frac{1}{T}
\left(
\mathbf{1}[i=j]-q_i^{(T)}
\right).
$$

Because the teacher probabilities sum to one,

$$
\begin{aligned}
\frac{\partial\mathcal{L}_{\mathrm{soft}}}{\partial z_i}
&=
-\sum_j p_j^{(T)}
\frac{\partial\log q_j^{(T)}}{\partial z_i}\\
&=
\frac{1}{T}
\left(
q_i^{(T)}-p_i^{(T)}
\right).
\end{aligned}
$$

This gives one explicit factor of \\(1/T\\). A second factor appears because the teacher and student distributions themselves become closer as the temperature rises.

Softmax is invariant to adding the same constant to every logit, so define centered logits

$$
\tilde z_i=z_i-\bar z,
\qquad
\tilde v_i=v_i-\bar v,
$$

for which \\(\sum_i\tilde z_i=\sum_i\tilde v_i=0\\). When \\(T\\) is large relative to the logit magnitudes,

$$
\exp(\tilde z_i/T)
=
1+\frac{\tilde z_i}{T}
+O(T^{-2}).
$$

For \\(N\\) classes, the centered first-order terms cancel in the denominator, giving

$$
q_i^{(T)}
=
\frac{1}{N}
+
\frac{\tilde z_i}{NT}
+
O(T^{-2}),
\qquad
p_i^{(T)}
=
\frac{1}{N}
+
\frac{\tilde v_i}{NT}
+
O(T^{-2}).
$$

Therefore,

$$
q_i^{(T)}-p_i^{(T)}
=
\frac{\tilde z_i-\tilde v_i}{NT}
+
O(T^{-2}),
$$

and the soft-loss gradient becomes

<div class="equation-note">
<span class="equation-label">High-temperature gradient</span>

$$
\frac{\partial\mathcal{L}_{\mathrm{soft}}}{\partial z_i}
=
\frac{\tilde z_i-\tilde v_i}{NT^2}
+
O(T^{-3}).
$$

The raw gradient thus decays approximately as 1/T². Multiplying the soft loss by T² restores its leading-order scale.
</div>

A binary example makes the effect concrete. Let the teacher logits be \\(v=[2,0]\\) and the student logits be \\(z=[1,0]\\). At \\(T=1\\),

$$
p_1^{(1)}\approx0.881,
\qquad
q_1^{(1)}\approx0.731,
\qquad
\frac{\partial\mathcal{L}_{\mathrm{soft}}}{\partial z_1}
\approx-0.150.
$$

At \\(T=10\\), the distributions are much softer:

$$
p_1^{(10)}\approx0.550,
\qquad
q_1^{(10)}\approx0.525,
$$

so

$$
\frac{\partial\mathcal{L}_{\mathrm{soft}}}{\partial z_1}
=
\frac{0.525-0.550}{10}
\approx-0.0025.
$$

The exact finite-temperature ratio need not be precisely \\(T^{-2}\\), but the high-temperature derivation explains the dominant scaling. Multiplying by \\(T^2=100\\) restores the gradient to the same general range as the hard-label signal. At inference time, the distilled student returns to \\(T=1\\).

These components should not be treated as isolated tricks. Initialization determines signal scale at the start of training; activation functions determine local derivatives; normalization and residual connections alter conditioning across depth; and the optimizer determines how gradients accumulate into parameter updates. The later ability to stack many Transformer blocks depended on this entire optimization infrastructure.

## 5. Convolutional Networks and the Revival of Deep Learning

Convolutional networks were not direct predecessors of language models, but they demonstrated that end-to-end representation learning could scale reliably with large datasets and GPUs. A two-dimensional convolution has the general form

$$
h_{i,j,k}
=
\phi\!\left(
b_k+
\sum_{u,v,c}K_{u,v,c,k}\,x_{i+u,j+v,c}
\right).
$$

Local connectivity and weight sharing encode translation structure while greatly reducing the number of parameters. From LeNet to [AlexNet (2012)](https://proceedings.neurips.cc/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html), computer vision established an engineering paradigm later inherited by language modeling: large datasets, GPU training, end-to-end objectives, deep representations, and reproducible optimization recipes.

The significance of AlexNet therefore extends beyond image classification. It showed that when model architecture, data scale, computing platforms, and training methods advance together, neural networks can replace traditional pipelines built around manually engineered features.

## 6. Language Models: From Counts to Continuous Representations

The purpose of a language model is to assign a probability to a sequence of symbols \\(w_{1:T}\\). By the chain rule of probability,

<div class="equation-note">
<span class="equation-label">Autoregressive factorization</span>

$$
P(w_{1:T})
=
\prod_{t=1}^{T}P(w_t\mid w_{<t}).
$$

This factorization remains the fundamental objective of autoregressive language models. Architectures have changed repeatedly, but the statistical problem of predicting the next symbol from its history has remained constant.
</div>

Traditional \\(n\\)-gram models use a finite-order Markov assumption:

$$
P(w_t\mid w_{<t})
\approx
P(w_t\mid w_{t-n+1:t-1}).
$$

Their parameters are usually estimated from corpus counts, with smoothing used to handle unseen combinations. Their fundamental difficulty is the sparsity of discrete contexts: two contexts that are semantically similar but lexically different cannot naturally share statistical strength.

[Bengio et al. (2003)](https://www.jmlr.org/papers/v3/bengio03a.html) introduced a neural probabilistic language model that maps each word to a continuous vector and uses a feed-forward network to predict the next word. Given an embedding matrix \\(E\\), a fixed-window context can be written as

$$
c_t=[Ew_{t-n+1};\ldots;Ew_{t-1}],
\qquad
h_t=\tanh(W_c c_t+b_c),
$$

$$
P(w_t=j\mid c_t)
=
\frac{\exp(u_j^{\top}h_t+b_j)}
{\sum_{k=1}^{|V|}\exp(u_k^{\top}h_t+b_k)}.
$$

Maximum-likelihood training is equivalent to minimizing token-level cross-entropy:

$$
\mathcal{L}_{\mathrm{LM}}
=
-\sum_{t=1}^{T}\log P_{\theta}(w_t\mid w_{<t}).
$$

The corresponding perplexity is

$$
\operatorname{PPL}
=
\exp\!\left(
-\frac{1}{T}\sum_{t=1}^{T}
\log P_{\theta}(w_t\mid w_{<t})
\right).
$$

Continuous representations allow contexts with similar semantic or syntactic roles to share parameters. This was the decisive transition from count-based statistical language models to neural language models. A fixed context window, however, still cannot represent dependencies of arbitrary length.

## 7. Recurrent Networks: Compressing History into State

A recurrent neural network processes a variable-length sequence through a recursively updated state:

$$
h_t=\phi(W_xx_t+W_hh_{t-1}+b_h),
\qquad
P(w_{t+1}\mid w_{\le t})=\operatorname{softmax}(W_oh_t+b_o).
$$

The state \\(h_t\\) is expected to summarize all preceding inputs. This is an important generalization beyond fixed-window models. Training, however, requires backpropagation through time, so its gradients contain long products of Jacobians. Information that a model can preserve in principle is not necessarily information that optimization can learn in practice.

### LSTM: Explicit Control over Writing and Forgetting

[Hochreiter and Schmidhuber (1997)](https://direct.mit.edu/neco/article/9/8/1735/6109/Long-Short-Term-Memory) introduced the LSTM, which controls information flow through gates. A common modern formulation is

$$
i_t=\sigma(W_ix_t+U_ih_{t-1}+b_i),
\qquad
f_t=\sigma(W_fx_t+U_fh_{t-1}+b_f),
$$

$$
o_t=\sigma(W_ox_t+U_oh_{t-1}+b_o),
\qquad
\tilde c_t=\tanh(W_cx_t+U_ch_{t-1}+b_c),
$$

$$
c_t=f_t\odot c_{t-1}+i_t\odot\tilde c_t,
\qquad
h_t=o_t\odot\tanh(c_t).
$$

The forget gate \\(f_t\\) determines how much old memory to preserve, the input gate \\(i_t\\) determines how much new content to write, and the output gate \\(o_t\\) determines how much internal memory to expose as the current state. The most important feature is the additive update of the cell state. Compared with the repeated nonlinear transformations of a standard RNN, it provides a more direct path for gradient propagation.

LSTMs remained central to speech recognition, machine translation, and language modeling for many years. Yet they retained an unavoidable sequential dependency: \\(h_{t-1}\\) must be computed before \\(h_t\\). This dependence later became a major obstacle to large-scale parallel training.

## 8. Word Vectors and Distributed Semantics

The distributional hypothesis holds that a word's meaning can be characterized by the contexts in which it occurs. Neural language models already learned word vectors implicitly, while [Word2Vec (2013)](https://proceedings.neurips.cc/paper/2013/hash/9aa42b31882ec039965f3c4923ce901b-Abstract.html) reduced representation learning to an efficient local prediction task.

The idealized skip-gram objective is

$$
\max_{\theta}
\sum_{t=1}^{T}
\sum_{-m\le j\le m,\,j\ne 0}
\log P(w_{t+j}\mid w_t).
$$

To avoid computing a softmax over the entire vocabulary, negative sampling turns each update into a binary classification problem:

$$
\log\sigma(v_{w_o}^{\top}v_{w_c})
+
\sum_{k=1}^{K}
\mathbb{E}_{w_k\sim P_n}
\left[
\log\sigma(-v_{w_k}^{\top}v_{w_c})
\right].
$$

Here \\(w_c\\) is the center word, \\(w_o\\) is an observed context word, and \\(w_k\\) is a negative sample. This method made large-scale word-vector training economical and established semantic relations in vector spaces as a standard representational framework in NLP.

Its limitation is equally clear: each word usually receives only one static vector. The meaning of the same word therefore cannot change across sentences. Contextual representations require a sequence model to participate in the computation.

## 9. Sequence-to-Sequence Learning: From Representing Sequences to Generating Them

[Sequence to Sequence Learning (2014)](https://arxiv.org/abs/1409.3215) used one recurrent network to encode an input and another to generate an output autoregressively. For an input \\(x_{1:S}\\) and output \\(y_{1:T}\\), the model is

$$
h_s^{\mathrm{enc}}
=
f_{\mathrm{enc}}(x_s,h_{s-1}^{\mathrm{enc}}),
\qquad
c=h_S^{\mathrm{enc}},
$$

$$
P(y_{1:T}\mid x_{1:S})
=
\prod_{t=1}^{T}
P(y_t\mid y_{<t},c).
$$

The importance of this architecture is that it does not require separate output spaces for translation, summarization, or question answering. Instead, it unifies these tasks as conditional sequence generation. The entire input, however, is compressed into a single vector \\(c\\), creating a severe information bottleneck. As the input grows longer, it becomes increasingly difficult for the encoder to preserve every relevant detail in one fixed representation.

## 10. Attention: From Fixed Compression to Content Addressing

[Bahdanau, Cho, and Bengio (2014)](https://arxiv.org/abs/1409.0473) proposed reading all encoder states anew when generating each output symbol. Let \\(s_{t-1}\\) be the previous decoder state and \\(h_j\\) the \\(j\\)-th encoder state. The alignment score is

<div class="equation-note">
<span class="equation-label">Additive attention</span>

$$
e_{t,j}
=
v_a^{\top}\tanh(W_s s_{t-1}+W_h h_j),
$$

$$
\alpha_{t,j}
=
\frac{\exp(e_{t,j})}
{\sum_{k=1}^{S}\exp(e_{t,k})},
\qquad
c_t=\sum_{j=1}^{S}\alpha_{t,j}h_j.
$$

The context is no longer a fixed vector \\(c\\), but a step-dependent vector \\(c_t\\). The weights \\(\alpha_{t,j}\\) perform content-based addressing over input positions for the current output.
</div>

Attention solved two important problems. First, information no longer had to pass entirely through the encoder's final state. Second, the model could learn a soft alignment between input and output. At this stage, however, attention was still attached to an RNN encoder and an RNN decoder. State updates remained sequential, and long-range information still had to travel partly through recurrent paths.

## 11. By 2016, the Necessary Components Were in Place

By 2016, most of the foundations of modern language models had already appeared:

1. **Probabilistic objective:** A language sequence could be modeled as a product of conditional probabilities and trained with cross-entropy.
2. **Differentiable representations:** Words, contexts, and hidden states could be mapped into continuous vector spaces.
3. **Credit assignment:** Backpropagation could train computation graphs composed of many differentiable modules.
4. **Stable deep training:** Initialization, non-saturating activations, normalization, residual connections, gradient clipping, and adaptive optimizers had matured.
5. **Sequential state:** RNNs and LSTMs could represent variable-length histories and gated memory.
6. **A unified generation interface:** Sequence-to-sequence learning converted multiple NLP tasks into conditional generation.
7. **Content addressing:** Attention allowed a model to access different input positions according to its current need.
8. **Open-vocabulary modeling:** [BPE subword segmentation (2016)](https://aclanthology.org/P16-1162/) established a compromise between characters and words, reducing both out-of-vocabulary failures and the need for extremely large vocabularies.

<div class="synthesis" markdown="1">
### The Remaining Structural Problems

These components were sufficient to build powerful sequence models, but three difficulties remained. First, recurrent state prevented full parallelization across sequence positions. Second, two distant positions were still connected by a long computational path. Third, the encoder, decoder, and attention mechanism were composed of different kinds of operations, producing a complex architecture that was costly to scale.

The next step was therefore not to reinvent the language-modeling objective, but to reorganize the existing components: preserve attention, representation learning, residual connections, normalization, and feed-forward networks while removing recurrence. The Transformer emerged in 2017 under precisely these technical conditions.
</div>

## 12. Timeline of Key Milestones

| Year | Work | Historical role |
|---|---|---|
| 1943 | McCulloch–Pitts neuron | Expressed a neuron as a composable weighted logical unit |
| 1950 | Turing, *Computing Machinery and Intelligence* | Turned machine intelligence into a concrete and testable question |
| 1958 | Perceptron | Introduced an early data-driven rule for learning weights |
| 1986 | Backpropagation | Enabled multilayer networks to learn internal representations |
| 1997 | LSTM | Addressed long-term dependencies through gates and additive memory |
| 2003 | Neural probabilistic language model | Jointly learned word embeddings and next-word prediction |
| 2010 | Xavier initialization | Improved the scale of signals and gradients in deep networks |
| 2011 | ReLU | Provided a simple, non-saturating, piecewise-linear activation |
| 2012 | AlexNet | Demonstrated the scaling paradigm of deep networks, GPUs, and large datasets |
| 2013 | Word2Vec | Established large-scale distributed word representations as a standard component |
| 2014 | Seq2Seq, attention, Adam, dropout | Unified conditional generation and substantially improved optimization and generalization |
| 2015 | BatchNorm, He initialization, knowledge distillation | Stabilized deep training and introduced soft-target transfer from large teachers to smaller students |
| 2016 | ResNet, LayerNorm, BPE, GELU | Supplied residual paths, normalization, subwords, and activation functions for deep sequence architectures |

## Conclusion

The history before the Transformer shows that artificial intelligence did not advance through a simple succession in which one architecture replaced another. A more accurate account is that problem formulations, mathematical tools, and engineering mechanisms accumulated over time and were eventually recombined. Symbolic AI supplied the language of states, actions, planning, and structured reasoning. Statistical learning established the principle of estimating models from data. Neural networks provided differentiable representations. Backpropagation solved internal credit assignment. The infrastructure of deep learning made large-scale optimization practical. RNNs, LSTMs, sequence-to-sequence learning, and attention progressively defined the central problems of sequence modeling.

The value of understanding this history is not merely to identify who introduced a particular module first. It allows us to distinguish advances caused by new modeling assumptions from those enabled by improved optimization, greater computational and data scale, or the recombination of existing ideas in a new system. The same distinction remains essential when evaluating research on large language models today.

<div class="references" markdown="1">
## Further Reading

1. Stuart Russell and Peter Norvig. [*Artificial Intelligence: A Modern Approach*, Chapter 1](https://aima.cs.berkeley.edu/contents.htm). A broad history covering symbolic AI, expert systems, probabilistic reasoning, machine learning, and deep learning.
2. Ian Goodfellow, Yoshua Bengio, and Aaron Courville. [*Deep Learning*, Chapter 1](https://www.deeplearningbook.org/contents/intro.html). An account organized around three waves of neural networks, increasing data scale, and computing infrastructure.
3. Jürgen Schmidhuber. [*Deep Learning in Neural Networks: An Overview*](https://arxiv.org/abs/1404.7828). A technically detailed historical review; its claims about priority should be read alongside other histories.
4. Yann LeCun, Yoshua Bengio, and Geoffrey Hinton. [*Deep Learning*](https://www.nature.com/articles/nature14539), *Nature*, 2015. A concise review of representation learning, convolutional networks, recurrent networks, and backpropagation.
5. Yoshua Bengio et al. [*A Neural Probabilistic Language Model*](https://www.jmlr.org/papers/v3/bengio03a.html), *JMLR*, 2003.
6. Sepp Hochreiter and Jürgen Schmidhuber. [*Long Short-Term Memory*](https://direct.mit.edu/neco/article/9/8/1735/6109/Long-Short-Term-Memory), *Neural Computation*, 1997.
7. Ilya Sutskever, Oriol Vinyals, and Quoc V. Le. [*Sequence to Sequence Learning with Neural Networks*](https://arxiv.org/abs/1409.3215), 2014.
8. Dzmitry Bahdanau, Kyunghyun Cho, and Yoshua Bengio. [*Neural Machine Translation by Jointly Learning to Align and Translate*](https://arxiv.org/abs/1409.0473), 2014.
9. Geoffrey Hinton, Oriol Vinyals, and Jeff Dean. [*Distilling the Knowledge in a Neural Network*](https://arxiv.org/abs/1503.02531), 2015.
</div>
  </div>
</div>
