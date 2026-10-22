Welcome to my portfolio! I'm a credit risk modeler and product developer at KPMG, where I build and own analytics tools. My work sits at the intersection of finance, risk management and data science: leading model development teams, and designing the products that make that work faster.

(571) 271-2018 • [benuehlinger@gmail.com](mailto:benuehlinger@gmail.com) • McLean, VA

---

## **Education**

- **M.S. in Business Analytics**, William & Mary *(December 2024)* *4.00 GPA*
- **B.B.A in Finance**, James Madison University *(May 2021)* *3.61 GPA*

---

## **Work Experience**

**Modeling & Analytics Consultant @ KPMG US** *(June 2021 – Present)*  
- Manage two large staff augmentation workstreams within a large U.S. bank's quantitative office, leading teams of 12 and 7 that build models for the Credit Loss and Wholesale Risk Rating teams. The role calls for daily stakeholder engagement and hands-on technical expertise.
- Developed CECL C&I Probability of Default, Prepayment and UAD models for a midwest regional bank in DataBricks (Python), conducting daily coding workshops with the data science team to showcase progress.
- Validated CECL ensemble credit card model (PD, EAD, LGD), conducting sensitivity analyses, benchmarking, and stability tests for largest US credit union
- Designed GenAI risk-tiering framework and Retrieval Augmented Generation (RAG) model risk standard for a mid-sized midwest bank
- Led internal AI/ML model risk management research, resulting in at least three business opportunities and RFP wins
- Implemented parameter-efficient tuning (LoRA, QLoRA, DoRA) on DistilBERT models, presenting results to internal leadership in education sessions 
- Designed synthetic transaction testing for two machine learning models for a major tech client.
- Collaborate with multiple large banks throughout quarterly CECL accounting process to review entity's ongoing performance monitoring

---

## **Products Built at KPMG**

**ReserveIQ**  
- Built for financial due diligence (FDD) engagements where a lender needs a credit mark on a loan portfolio, which means building fast credit loss models on tight timelines. Much of that work repeats from deal to deal, so I turned it into a low-code tool.
- Built a Python/Streamlit reserve analytics app that ingests any bank's loan tape through schema-flexible column mapping. I chose Streamlit because the modeling team already works in Python, so analysts get a point-and-click interface on top of the same code without a separate front-end build.
- Fits panel logit PD (statsmodels) and LGD models and computes ECL = PD × LGD × balance.
- Stress-tests with Federal Reserve CCAR scenario paths joined to FRED macro history. The app then builds a PowerPoint deck (Plotly, python-pptx), with an LLM (gpt-oss-120b on Azure AI Foundry) drafting the chart narratives. The workflow cuts reserve analysis from 4 weeks to 4 days by eliminating most manual model-building hours, the main cost on FDD engagements.
- Presented firm-wide at an all-hands.
- Deployed as a Docker container on Azure Container Apps with Azure AD sign-in, per-user data separation and GitHub Actions CI/CD.

**CreditIQ**  
- Rebuilt ReserveIQ from a Streamlit prototype into a full model development workbench for consumer, mortgage and commercial real estate books.
- Moved the UI to React/TypeScript (Vite, Tailwind, ECharts, Zustand, TanStack Query) on a FastAPI backend, so heavy model fits run only when a user asks and switching views costs no compute.
- Every model is identified by a hash of its specification and data, making results cacheable and saved versions immutable and exactly reproducible.
- Automated variable selection, optimal binning, loan tape ingestion with validation, backtesting, and PD + LGD projection through 2026 Fed supervisory scenarios with FRED macro history. Backed by a backend test suite and browser tests.
- Presented to C-suite leaders at a national banking industry conference.
- Deployed as a Docker container on Azure Container Apps with Azure AD single sign-on, per-user data isolation and YAML-versioned configs.

<div class="ciq">
<style>
.ciq{margin:14px 0 6px}
.ciq-frame{position:relative;border-radius:8px;overflow:hidden;box-shadow:0 1px 3px rgba(0,0,0,.12),0 6px 18px rgba(0,0,0,.08)}
.ciq-track{display:flex;overflow-x:auto;scroll-snap-type:x mandatory;scroll-behavior:smooth;scrollbar-width:none}
.ciq-track::-webkit-scrollbar{display:none}
.ciq-slide{flex:0 0 100%;scroll-snap-align:start;aspect-ratio:1.94;background:#0d1117}
.ciq-slide img{display:block;width:100%;height:100%;object-fit:cover;object-position:top left;border:0;max-width:none}
.ciq-arrow{position:absolute;top:50%;transform:translateY(-50%);width:30px;height:30px;border:0;border-radius:50%;background:rgba(255,255,255,.85);color:#222;font-size:18px;line-height:30px;padding:0;cursor:pointer;opacity:0;transition:opacity .2s;box-shadow:0 1px 4px rgba(0,0,0,.3)}
.ciq-frame:hover .ciq-arrow,.ciq-arrow:focus{opacity:1}
@media (hover:none){.ciq-arrow{opacity:.85}}
.ciq-prev{left:8px}.ciq-next{right:8px}
.ciq-meta{display:flex;justify-content:space-between;align-items:baseline;gap:12px;margin-top:8px;font-size:13px;line-height:1.45;color:#727272}
.ciq-meta b{color:#222;font-weight:600}
.ciq-count{white-space:nowrap;font-variant-numeric:tabular-nums;color:#aaa;font-size:12px}
.ciq-note{font-size:12px;color:#aaa;margin:2px 0 0}
</style>
<div class="ciq-frame">
<div class="ciq-track">
<a class="ciq-slide" href="assets/img/creditiq/01.jpg" target="_blank" data-t="Portfolio roll-up" data-c="Champion models across three books, stressed under the Fed severely adverse scenario."><img src="assets/img/creditiq/01.jpg" alt="CreditIQ Portfolio roll-up" loading="lazy"></a>
<a class="ciq-slide" href="assets/img/creditiq/02.jpg" target="_blank" data-t="Panel" data-c="Realized default rates over time, with automated data integrity checks."><img src="assets/img/creditiq/02.jpg" alt="CreditIQ Panel" loading="lazy"></a>
<a class="ciq-slide" href="assets/img/creditiq/03.jpg" target="_blank" data-t="Macro variable search" data-c="650 candidate macro terms ranked against the default rate."><img src="assets/img/creditiq/03.jpg" alt="CreditIQ Macro variable search" loading="lazy"></a>
<a class="ciq-slide" href="assets/img/creditiq/04.jpg" target="_blank" data-t="PD model" data-c="Fitted specification with coefficients, standard errors, VIF and contribution."><img src="assets/img/creditiq/04.jpg" alt="CreditIQ PD model" loading="lazy"></a>
<a class="ciq-slide" href="assets/img/creditiq/05.jpg" target="_blank" data-t="Scenarios" data-c="ECL attribution bridge and cumulative expected loss over the horizon."><img src="assets/img/creditiq/05.jpg" alt="CreditIQ Scenarios" loading="lazy"></a>
<a class="ciq-slide" href="assets/img/creditiq/06.jpg" target="_blank" data-t="Versions" data-c="Saved models with reproducible IDs and a lineage graph."><img src="assets/img/creditiq/06.jpg" alt="CreditIQ Versions" loading="lazy"></a>
</div>
<button type="button" class="ciq-arrow ciq-prev" aria-label="Previous screenshot">&#8249;</button>
<button type="button" class="ciq-arrow ciq-next" aria-label="Next screenshot">&#8250;</button>
</div>
<div class="ciq-meta"><span class="ciq-cap"></span><span class="ciq-count"></span></div>
<p class="ciq-note">Synthetic demonstration data. Click a screenshot to open it full size.</p>
<script>
(function(){var c=document.currentScript.parentNode,t=c.querySelector('.ciq-track'),s=t.children,cap=c.querySelector('.ciq-cap'),n=c.querySelector('.ciq-count'),k=0;
function show(){var e=s[k];cap.innerHTML='<b>'+e.dataset.t+'.</b> '+e.dataset.c;n.textContent=(k+1)+' / '+s.length}
function go(i){k=(i+s.length)%s.length;t.scrollTo({left:k*t.clientWidth});show()}
c.querySelector('.ciq-prev').onclick=function(){go(k-1)};c.querySelector('.ciq-next').onclick=function(){go(k+1)};
t.addEventListener('scroll',function(){clearTimeout(t._m);t._m=setTimeout(function(){k=Math.round(t.scrollLeft/t.clientWidth);show()},120)});show();})();
</script>
</div>


**DecisionIQ**  
- Built an AI infrastructure decision-modeling tool for a major tech company with heavy AI investment exposure, helping leadership decide whether acquisitions are feasible and, if so, which targets make sense.
- Capacity model: projects AI capex commitments against ad revenue through free cash flow to M&A capacity, showing how much room the company has to act under each internal scenario.
- Contagion model: maps deals and dependencies across the AI ecosystem as a network graph (NetworkX) and scores each entity on opportunity and threat, flagging which targets strengthen the company's position and which carry spillover risk.
- Runs both models across scenario sweeps, replacing single-point forecasts with a quantified downside view on multibillion-dollar capex. Built in Python/Streamlit on Azure.
- Presented twice to the company's Chief Accounting Officer.

---

## **Personal and Educational Projects**

**Reverse-Engineering CMS Star Algorithm** *December 2024, William & Mary Capstone*  
- The CMS Star Rating quality metric from CMS that clusters hospitals into measure groups, and scores them on a scale of 1-to-5.
- Using publicly available information, our three-person team replicated the rating algorithm for 4,000+ hospitals, used machine learning to identify key measures, and simulated future star rating changes to deliver insights to our client, Riverside Hospital.
- The project is posted on [GitHub](https://github.com/benuehlinger/WM-Capstone).

**Low Rank Adaptation (LoRA) for Finetuning LLMs** *September 2024*  
- Performed research to understand how LoRA can make fine-tuning LLMs more efficient.
- The results are summarized in this [Medium post](https://medium.com/@benuehlinger/low-rank-adaptation-lora-for-fine-tuning-llms-2a04ba28b3a2), and the code is posted on [GitHub](https://github.com/benuehlinger/LoRA-finetune).

**COVID-19: A Black Swan?** *May 2021, James Madison Honors Capstone*  
- Applied Nassim Taleb’s tail-risk framework to assess the pandemic’s predictability and impact compared to other low-probability, high-impact events like 9/11 and the 2008 global financial crisis.  
- Performed cointegration tests and visually inspected returns of 11 SPDR Sector ETFs.
- [LinkedIn post](https://www.linkedin.com/posts/benuehlinger_covid-19-a-black-swan-activity-6805583797850005505-TC78?utm_source=share&utm_medium=member_desktop) with results.

---

Thank you for visiting my portfolio! I’m always looking to collaborate on interesting projects or discuss potential consulting opportunities. Let’s build something innovative together.

