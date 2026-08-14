

I build things that have to be fast. 
The rest of the time I'm on Codeforces at 2 a.m.

<div align="center"><img src="assets/rule.svg" alt="" width="100%" /></div>

### Now

Software Engineer Intern at **TIH — IIT Bombay**, teaching an NLP pipeline to read raw bank statements.
Open to software engineering internships.

<div align="center"><img src="assets/rule.svg" alt="" width="100%" /></div>

### Work

<details>
<summary><b>order-book-matching-engine</b> — the core of an electronic exchange, running in a browser tab</summary>

<br />

Built from published specifications — Selph, LOBSTER — with no reference implementation to lean on. Just the papers.

The book is an `std::map` price ladder over doubly-linked FIFO levels, with an `id → node` hash map alongside it. That combination buys **O(1) cancellation** and **O(log M) inserts**, which is what lets it sustain **~4M orders/sec at ~250 ns per order**. Eleven unit tests keep it honest.

Then I compiled it to WebAssembly with Emscripten and put a live visualizer on GitHub Pages, so the same low-latency C++ runs client-side.

`C++17` · `WebAssembly` · `Emscripten` · `CMake`

[→ repository](https://github.com/xaemonn/order-book-matching-engine)

</details>

<details>
<summary><b>eDAG-MEC</b> — research that had only ever been simulated, moved into the kernel</summary>

<br />

Dependency-aware Mobile Edge Computing, accelerated by moving task routing and caching into the Linux kernel with **eBPF** — realising on real hardware what prior work assumed only in simulation.

kube-proxy and iptables came out; **O(1) kernel hash-map lookups** went in. On top of that sits a kernel-resident result cache with dependency-aware eviction driven by the task topology.

Benchmarked on a 3-node AWS EC2 cluster: up to **7.1× task speedup** and **~18× cache fan-out** over baseline.

`Golang` · `C` · `eBPF/XDP` · `Kubernetes` · `AWS`

[→ repository](https://github.com/xaemonn/dpls-xdp)

</details>

<details>
<summary><b>Credit Mitra</b> — reading bank statements the way an analyst would</summary>

<br />

An NLP pipeline that parses raw PDF bank statements and classifies transactions through LLM-powered extraction, which removed most of the manual data-cleaning that used to sit in front of the analysis.

A FastAPI backend feeds a React dashboard, so institutions can ask it for category breakdowns and merchant/payee insights and get answers in under a second.

Built during my internship at Technology Innovation Hub, IIT Bombay.

`Python` · `FastAPI` · `React` · `LLMs`

[→ repository](https://github.com/xaemonn/Credit_Mitra_IITB)

</details>

<br />

Daily practice lives in [xmon-leetcode](https://github.com/xaemonn/xmon-leetcode), [CSES-problem-set](https://github.com/xaemonn/CSES-problem-set) and [CF_Solutions](https://github.com/xaemonn/CF_Solutions).

<div align="center"><img src="assets/rule.svg" alt="" width="100%" /></div>

### Selected results

> **39** — global rank, ICPC AlgoQueen 2025. And 398 in the Prelims.<br />
> **1200+** — algorithm problems solved across competitive platforms.<br />
> **1531** — peak Codeforces rating. Specialist.<br />
> **2000+** — LeetCode rating. Knight.<br />
> **Top 300** — nationwide, Amazon HackOn 2026. Top 3000 for MLSS, from 1,34,421 applicants.<br />
> **Top 10** — of 550+ teams at SheBuilds Hacks '25. Finalist at HackVega '25 by Myntra.<br />
> **Selected** — Microsoft Code Without Barriers mentee, 2025.

<div align="center"><img src="assets/rule.svg" alt="" width="100%" /></div>

### Elsewhere

[Email](mailto:dishakwatra01@gmail.com) · [LinkedIn](https://www.linkedin.com/in/disha-kawatra) · [LeetCode](https://leetcode.com/u/dishakwatra01) · [Codeforces](https://codeforces.com/profile/dishakwatra)

<br />

