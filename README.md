# Hi, I'm Nikita

I'm a graduate student in Northeastern University's MS in Project Management (Analytics concentration) in Boston, and a research assistant at the D'Amore-McKim School of Business. Before graduate school, I spent nearly three years at Viacom18 in Mumbai, using audience data to plan TV programming.

I like questions with messy data behind them, and I build my projects so anyone can check the answer: each data analysis below rebuilds its results from public data with one command, and an automated test checks every published figure.

**Looking for a Spring 2027 co-op (January start)** in product, program or project management, or analytics.

## Projects

Each project starts with a question anyone can follow. The short answer is here; the full method, charts and code are one click away.

### [What is a show actually worth to a streaming service?](https://github.com/tiwari-nikita/streaming-catalog-value)

Netflix publishes how many hours people watched every title. Across seven reports and almost 29,000 titles: about half of all viewing is of shows licensed from other studios, new originals lose over 90% of their daily viewing after launch, and next half-year's viewing can be forecast with a typical error of about 25%, beating simple rules of thumb.

<sub>**Under the hood:** title-by-half-year panel of 97,736 observations from Netflix's engagement reports (2023–2026), launch decay, retention by segment, and a demand forecast tested on a held-out half against naive baselines. Python, pandas, scikit-learn. `verify.py` checks all 10 published figures.</sub>

### [What's inside a grid battery's price, and do grid projects ever get built?](https://github.com/tiwari-nikita/grid-storage-analysis)

Using only the prices on Tesla's website, I recovered the exact formula behind Megapack pricing (it matches all 18 prices), and found that 91% of the price is the part exposed to tariffs and Chinese battery supply. Of 20,087 requests to connect new projects to the US grid, only about 1 in 5 is built within ten years, and an identical battery project is about 8 times as likely to be built in Texas as in California.

<sub>**Under the hood:** price decomposition fitted at R² = 1.000000, a cost trace from raw materials to delivered system, and a competing-risks survival analysis (Aalen-Johansen, written from scratch) of LBNL's interconnection-queue data. Python. `verify.py` checks all 29 published claims plus a 13-check independent audit.</sub>

### [Did charging drivers to enter Manhattan cut traffic?](https://github.com/tiwari-nikita/nyc-congestion-pricing)

Yes, modestly. After congestion pricing began in January 2025, traffic through the tunnels into the zone fell 2–4% compared with similar bridges, drivers didn't simply reroute, and the drop held into a second year. Pretending other bridges were tolled, or that the toll started on other dates, never produced an effect as large.

<sub>**Under the hood:** difference-in-differences on 1,342 days of MTA bridge and tunnel crossings, with permutation inference, an event study, a diversion test and an explicit pre-trend check. Python. `verify.py` checks all 10 published figures.</sub>

### [Do companies explain how they keep AI under control?](https://github.com/tiwari-nikita/ai-oversight-gap)

Rarely. In 2025, about half of US public companies' annual reports mentioned AI, but fewer than 2 in 100 described governing it. Set against 1,689 real AI incidents, 98% of the harm happened after a system was already in use, and three kinds of safeguard would cover about 71% of it.

<sub>**Under the hood:** every 10-K filed 2019 to September 2026 via SEC EDGAR full-text search, the AI Incident Database classified with the MIT AI Risk Repository taxonomy, and a published mapping to NIST AI RMF safeguards. Python. `verify.py` checks all 12 published figures.</sub>

### [Which free AI model should I use, for the things I actually ask?](https://github.com/tiwari-nikita/llm-eval-harness)

Public leaderboards can't tell you which AI is best for your own questions. This tool sends my real questions to free AI models, has me pick the better answer without knowing which model wrote it, and turns those picks into a recommendation for each kind of question. It also found that the AI "graders" most evaluations rely on disagree about which model wins, so it measures them against a real person's choices.

<sub>**Under the hood:** blind pairwise preference with Bradley–Terry ranking and bootstrapped confidence, privacy gates enforced in code (nothing is sent without explicit approval), citation checks against OpenAlex and Crossref, and a second LLM grader from an unrelated model family. Python. 240+ tests, every network call mocked.</sub>

## How I work

- **Real public data only**, with each source file fingerprinted so an analysis can't silently run on different data.
- **Every published number has a test.** One command rebuilds the results and fails if any figure changes.
- **Limitations stated up front**, not buried in a footnote.

## Contact

[LinkedIn](https://www.linkedin.com/in/nikitatiwari-/)
