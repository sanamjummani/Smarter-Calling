<!-- ============================================================
     SMARTER CALLING — README
     Sana Majeed · Purdue University
     ============================================================ -->

<div align="center">

<br/>

<table width="100%" cellspacing="0" cellpadding="0" style="background:#0D1E35;border:1px solid #C9A84C;border-radius:4px;max-width:900px">
<tr>
<td style="padding:36px 40px 28px 40px">

<p style="font-family:monospace;font-size:11px;letter-spacing:3px;color:#2D8C8C;text-transform:uppercase;margin:0 0 14px 0">
&mdash;&nbsp; Predictive Targeting · Bank Telemarketing · Logistic Regression
</p>

<h1 style="font-size:38px;font-weight:800;color:#FFFFFF;margin:0 0 6px 0;line-height:1.1">
Smarter Calling
</h1>

<p style="font-size:16px;color:#C9A84C;font-style:italic;margin:0 0 16px 0">
How predictive targeting cut call volume by 44% while growing profit by 11%
</p>

<p style="font-size:14px;color:#B0B8C8;line-height:1.75;margin:0 0 24px 0;max-width:680px">
A Portuguese bank runs outbound calls to sell term deposit subscriptions. Every call costs $20. Every conversion earns $200. The instinct is to call everyone. This project shows why that instinct is wrong — and builds a logistic regression model that turns a spray-and-pray campaign into a precision strategy.
</p>

<!-- STAT STRIP -->
<table cellspacing="0" cellpadding="0" width="100%">
<tr>
<td align="center" width="25%" style="padding:16px 8px;border-top:1px solid rgba(201,168,76,0.25);border-right:1px solid rgba(201,168,76,0.15)">
  <div style="font-size:30px;font-weight:800;color:#C9A84C;line-height:1">+11%</div>
  <div style="font-size:11px;color:#8A94A6;margin-top:5px;letter-spacing:0.04em">Profit improvement</div>
</td>
<td align="center" width="25%" style="padding:16px 8px;border-top:1px solid rgba(201,168,76,0.25);border-right:1px solid rgba(201,168,76,0.15)">
  <div style="font-size:30px;font-weight:800;color:#C9A84C;line-height:1">−44%</div>
  <div style="font-size:11px;color:#8A94A6;margin-top:5px;letter-spacing:0.04em">Fewer calls made</div>
</td>
<td align="center" width="25%" style="padding:16px 8px;border-top:1px solid rgba(201,168,76,0.25);border-right:1px solid rgba(201,168,76,0.15)">
  <div style="font-size:30px;font-weight:800;color:#C9A84C;line-height:1">90%</div>
  <div style="font-size:11px;color:#8A94A6;margin-top:5px;letter-spacing:0.04em">Sensitivity / Recall</div>
</td>
<td align="center" width="25%" style="padding:16px 8px;border-top:1px solid rgba(201,168,76,0.25)">
  <div style="font-size:30px;font-weight:800;color:#C9A84C;line-height:1">$9,800</div>
  <div style="font-size:11px;color:#8A94A6;margin-top:5px;letter-spacing:0.04em">Additional net profit</div>
</td>
</tr>
</table>

</td>
</tr>
</table>

<br/>

<!-- TOOL BADGES -->
<p>
<img src="https://img.shields.io/badge/Python-3.x-1B2A4A?style=flat-square&labelColor=0D1E35&color=C9A84C"/>
&nbsp;
<img src="https://img.shields.io/badge/Logistic_Regression-statsmodels-1B2A4A?style=flat-square&labelColor=0D1E35&color=2D8C8C"/>
&nbsp;
<img src="https://img.shields.io/badge/scikit--learn-ROC_AUC-1B2A4A?style=flat-square&labelColor=0D1E35&color=6B8F71"/>
&nbsp;
<img src="https://img.shields.io/badge/Dataset-UCI_ML_Repository-1B2A4A?style=flat-square&labelColor=0D1E35&color=8A94A6"/>
</p>

</div>

<br/>

---

## The Question

Conventional campaign strategy calls everyone and counts who converts. This project asks a different question: before you pick up the phone, what is the probability this specific customer will subscribe — and is that probability high enough to justify the cost of the call?

The answer comes from a logistic regression model trained on 5,466 cleaned customer records, evaluated against a profit-based decision rule derived mathematically from the cost structure before any modelling began.

---

<!-- FINDINGS SECTION -->
<table width="100%" cellspacing="0" cellpadding="0" style="border-left:3px solid #C9A84C;background:#0D1E35;margin:8px 0">
<tr><td style="padding:10px 16px">
<span style="font-family:monospace;font-size:10px;letter-spacing:3px;color:#C9A84C;text-transform:uppercase">Key Findings</span>
</td></tr>
</table>

<br/>

<table width="100%" cellspacing="0" cellpadding="0">

<tr valign="top">
<td width="52px" align="center" style="padding-top:4px">
<svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 30 L6 14 L14 19 L22 9 L30 15" stroke="#C9A84C" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M6 30 L30 30" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" opacity="0.3"/>
<circle cx="30" cy="15" r="2.5" fill="#C9A84C"/>
</svg>
</td>
<td style="padding:4px 0 20px 8px">
<strong>+11% profit from 44% fewer calls</strong><br/>
<span style="color:#8A94A6;font-size:13px">Targeted calling generated $99,740 net profit versus $89,940 from mass calling. Revenue dropped slightly. Cost dropped dramatically. The $9,800 gain came from concentration, not volume.</span>
</td>
</tr>

<tr valign="top">
<td width="52px" align="center" style="padding-top:4px">
<svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 28 L28 8" stroke="#8A94A6" stroke-width="1" stroke-dasharray="2.5 2" opacity="0.5"/>
<path d="M8 28 Q12 12 18 12 Q24 12 28 28" stroke="#C9A84C" stroke-width="1.8" fill="none" stroke-linecap="round"/>
<circle cx="18" cy="12" r="2.5" fill="#C9A84C" opacity="0.8"/>
<line x1="8" y1="28" x2="28" y2="28" stroke="#C9A84C" stroke-width="1" stroke-linecap="round" opacity="0.3"/>
</svg>
</td>
<td style="padding:4px 0 20px 8px">
<strong>Optimal cutoff = 10% — derived before any modelling</strong><br/>
<span style="color:#8A94A6;font-size:13px">From the economics alone: call when 200p − 20 > 0, which means p > 0.10. The decision rule was set mathematically before a single model was trained. This separates a profit-driven strategy from an arbitrary accuracy-optimised one.</span>
</td>
</tr>

<tr valign="top">
<td width="52px" align="center" style="padding-top:4px">
<svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="6" y="20" width="6" height="10" rx="1" fill="#C9A84C" opacity="0.3"/>
<rect x="15" y="13" width="6" height="17" rx="1" fill="#C9A84C" opacity="0.6"/>
<rect x="24" y="7" width="6" height="23" rx="1" fill="#C9A84C" opacity="0.9"/>
<line x1="6" y1="30" x2="30" y2="30" stroke="#C9A84C" stroke-width="0.8" opacity="0.25"/>
</svg>
</td>
<td style="padding:4px 0 20px 8px">
<strong>90% sensitivity — 9 in 10 subscribers correctly identified</strong><br/>
<span style="color:#8A94A6;font-size:13px">The model caught 651 of 723 actual subscribers in the test set. High sensitivity was the deliberate design goal: missing a subscriber costs $200, an unnecessary call costs only $20. The asymmetry in costs justifies the asymmetry in the metric.</span>
</td>
</tr>

<tr valign="top">
<td width="52px" align="center" style="padding-top:4px">
<svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
<circle cx="18" cy="18" r="11" stroke="#C9A84C" stroke-width="1.4" stroke-dasharray="3 2"/>
<circle cx="18" cy="18" r="6" stroke="#C9A84C" stroke-width="1.2"/>
<circle cx="18" cy="18" r="2" fill="#C9A84C"/>
</svg>
</td>
<td style="padding:4px 0 20px 8px">
<strong>Economic signals predict subscription better than demographics</strong><br/>
<span style="color:#8A94A6;font-size:13px">Consumer price index and employment variation rate were the top model drivers — ahead of age, job, or marital status. When the economy signals uncertainty, people avoid locking up savings. Macro context matters more than who someone is.</span>
</td>
</tr>

<tr valign="top">
<td width="52px" align="center" style="padding-top:4px">
<svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 26 C8 26 12 10 18 10 C24 10 28 26 28 26" stroke="#C9A84C" stroke-width="1.6" fill="none" stroke-linecap="round"/>
<path d="M8 26 L28 8" stroke="#8A94A6" stroke-width="1" stroke-dasharray="2 1.5" opacity="0.4"/>
<line x1="8" y1="26" x2="28" y2="26" stroke="#C9A84C" stroke-width="1" stroke-linecap="round" opacity="0.3"/>
<text x="12" y="19" font-size="6.5" fill="#C9A84C" font-family="monospace" font-weight="bold">0.74</text>
</svg>
</td>
<td style="padding:4px 0 20px 8px">
<strong>AUC = 0.74 — genuine predictive skill, not pattern matching</strong><br/>
<span style="color:#8A94A6;font-size:13px">The ROC curve confirms the model discriminates meaningfully across all possible cutoffs, not just the one we chose. A model with no skill would follow the diagonal at AUC = 0.50. Ours is well above it.</span>
</td>
</tr>

</table>

---

<!-- BUSINESS CASE TABLE -->
<table width="100%" cellspacing="0" cellpadding="0" style="border-left:3px solid #C9A84C;background:#0D1E35;margin:8px 0">
<tr><td style="padding:10px 16px">
<span style="font-family:monospace;font-size:10px;letter-spacing:3px;color:#C9A84C;text-transform:uppercase">Business Impact</span>
</td></tr>
</table>

<br/>

<table width="100%" cellspacing="0" cellpadding="0" style="border-collapse:collapse;font-size:13px">
<thead>
<tr style="background:#1B2A4A">
<th align="left" style="padding:10px 16px;color:#8A94A6;font-weight:500;font-family:monospace;font-size:11px;letter-spacing:0.08em;border-bottom:1px solid rgba(201,168,76,0.2)">METRIC</th>
<th align="right" style="padding:10px 16px;color:#8A94A6;font-weight:500;font-family:monospace;font-size:11px;letter-spacing:0.08em;border-bottom:1px solid rgba(201,168,76,0.2)">MASS CALLING</th>
<th align="right" style="padding:10px 16px;color:#C9A84C;font-weight:600;font-family:monospace;font-size:11px;letter-spacing:0.08em;border-bottom:1px solid rgba(201,168,76,0.2)">TARGETED</th>
<th align="right" style="padding:10px 16px;color:#8A94A6;font-weight:500;font-family:monospace;font-size:11px;letter-spacing:0.08em;border-bottom:1px solid rgba(201,168,76,0.2)">CHANGE</th>
</tr>
</thead>
<tbody>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04)">
<td style="padding:10px 16px;color:#B0B8C8">Customers called</td>
<td align="right" style="padding:10px 16px;color:#8A94A6">2,733</td>
<td align="right" style="padding:10px 16px;color:#FFFFFF;font-weight:600">1,523</td>
<td align="right" style="padding:10px 16px;color:#C4614A">−44%</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04);background:rgba(255,255,255,0.02)">
<td style="padding:10px 16px;color:#B0B8C8">Subscribers reached</td>
<td align="right" style="padding:10px 16px;color:#8A94A6">723</td>
<td align="right" style="padding:10px 16px;color:#FFFFFF;font-weight:600">651</td>
<td align="right" style="padding:10px 16px;color:#8A94A6">−10%</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04)">
<td style="padding:10px 16px;color:#B0B8C8">Revenue</td>
<td align="right" style="padding:10px 16px;color:#8A94A6">$144,600</td>
<td align="right" style="padding:10px 16px;color:#FFFFFF;font-weight:600">$130,200</td>
<td align="right" style="padding:10px 16px;color:#8A94A6">−10%</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04);background:rgba(255,255,255,0.02)">
<td style="padding:10px 16px;color:#B0B8C8">Calling cost</td>
<td align="right" style="padding:10px 16px;color:#8A94A6">$54,660</td>
<td align="right" style="padding:10px 16px;color:#FFFFFF;font-weight:600">$30,460</td>
<td align="right" style="padding:10px 16px;color:#6B8F71">−44%</td>
</tr>
<tr style="background:#1B2A4A">
<td style="padding:12px 16px;color:#FFFFFF;font-weight:700">Net Profit</td>
<td align="right" style="padding:12px 16px;color:#8A94A6;font-weight:600">$89,940</td>
<td align="right" style="padding:12px 16px;color:#C9A84C;font-weight:700;font-size:15px">$99,740</td>
<td align="right" style="padding:12px 16px;color:#6B8F71;font-weight:700">+11%</td>
</tr>
</tbody>
</table>

<br/>

> Revenue drops slightly. Cost drops dramatically. Profit rises. Concentrating effort on high-probability customers makes each call worth more.

---

<!-- WHAT'S IN THIS REPO -->
<table width="100%" cellspacing="0" cellpadding="0" style="border-left:3px solid #C9A84C;background:#0D1E35;margin:8px 0">
<tr><td style="padding:10px 16px">
<span style="font-family:monospace;font-size:10px;letter-spacing:3px;color:#C9A84C;text-transform:uppercase">What Is in This Repository</span>
</td></tr>
</table>

<br/>

<table width="100%" cellspacing="0" cellpadding="0">
<tr valign="top">
<td width="52px" align="center" style="padding-top:3px">
<svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="5" y="3" width="16" height="24" rx="1.5" stroke="#C9A84C" stroke-width="1.4"/>
<path d="M9 9 L17 9" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" opacity="0.5"/>
<path d="M9 13 L17 13" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" opacity="0.5"/>
<path d="M9 17 L14 17" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" opacity="0.5"/>
<circle cx="22" cy="22" r="6" fill="#0D1E35" stroke="#C9A84C" stroke-width="1.2"/>
<path d="M19.5 22 L21 23.5 L24.5 20" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
</td>
<td style="padding:2px 0 18px 10px">
<code>Smarter_Calling_Predictive_Targeting.ipynb</code><br/>
<span style="color:#8A94A6;font-size:13px">Full analysis in eleven sections. Profit cutoff derivation, data cleaning, logistic regression, confusion matrices, ROC curve, and the final profit comparison. Every section opens with the business question it answers before showing any code.</span>
</td>
</tr>
<tr valign="top">
<td width="52px" align="center" style="padding-top:3px">
<svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="3" y="5" width="24" height="18" rx="1.5" stroke="#C9A84C" stroke-width="1.4"/>
<line x1="3" y1="10" x2="27" y2="10" stroke="#C9A84C" stroke-width="1" opacity="0.4"/>
<rect x="7" y="13" width="7" height="6" rx="0.5" fill="#C9A84C" opacity="0.25"/>
<rect x="16" y="13" width="7" height="6" rx="0.5" fill="#C9A84C" opacity="0.15"/>
<line x1="12" y1="23" x2="18" y2="27" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" opacity="0.5"/>
<line x1="9" y1="27" x2="21" y2="27" stroke="#C9A84C" stroke-width="1.2" stroke-linecap="round" opacity="0.4"/>
</svg>
</td>
<td style="padding:2px 0 18px 10px">
<code>Smarter_Calling_Predictive_Targeting.pptx</code><br/>
<span style="color:#8A94A6;font-size:13px">Ten slides translating the model into a strategic narrative. Built for an account team or campaign planning audience — the emphasis is on what the findings mean for how sales teams should operate.</span>
</td>
</tr>
<tr valign="top">
<td width="52px" align="center" style="padding-top:3px">
<svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6 24 L6 8 L18 8 L24 14 L24 24 Z" stroke="#C9A84C" stroke-width="1.4" stroke-linejoin="round" fill="none"/>
<path d="M18 8 L18 14 L24 14" stroke="#C9A84C" stroke-width="1.2" stroke-linejoin="round" fill="none" opacity="0.5"/>
<path d="M10 17 L20 17" stroke="#C9A84C" stroke-width="1" stroke-linecap="round" opacity="0.4"/>
<path d="M10 20 L16 20" stroke="#C9A84C" stroke-width="1" stroke-linecap="round" opacity="0.4"/>
</svg>
</td>
<td style="padding:2px 0 18px 10px">
<code>data/README.md</code><br/>
<span style="color:#8A94A6;font-size:13px">Dataset documentation — what each variable means, where to download the source data, and how to place it in the folder so the notebook runs without changes.</span>
</td>
</tr>
</table>

---

<!-- METHODOLOGY -->
<table width="100%" cellspacing="0" cellpadding="0" style="border-left:3px solid #C9A84C;background:#0D1E35;margin:8px 0">
<tr><td style="padding:10px 16px">
<span style="font-family:monospace;font-size:10px;letter-spacing:3px;color:#C9A84C;text-transform:uppercase">How the Analysis Was Done</span>
</td></tr>
</table>

<br/>

The analysis starts with a step most projects skip: deriving the optimal cutoff before touching the model. From the cost structure ($200 revenue, $20 cost per call) it follows mathematically that a call is profitable when the predicted subscription probability exceeds 10%. That threshold was set in advance and held throughout.

From there — data cleaning to remove illiterate, defaulted, and unknown-status records, leaving 5,466 clean rows from 41,188. One-hot encoding for categoricals. A 50/50 train-test split with a fixed seed. Logistic regression via statsmodels for interpretable coefficients and p-values. Evaluation across sensitivity, specificity, precision, and ROC-AUC. Then a direct profit comparison between the targeted strategy and the mass calling baseline.

<br/>

<!-- METHODS TABLE -->
<table width="100%" cellspacing="0" cellpadding="0" style="border-collapse:collapse;font-size:13px">
<tr style="background:#1B2A4A;border-bottom:1px solid rgba(201,168,76,0.2)">
<th align="left" style="padding:9px 14px;color:#8A94A6;font-weight:500;font-family:monospace;font-size:10px;letter-spacing:0.1em;width:35%">COMPONENT</th>
<th align="left" style="padding:9px 14px;color:#8A94A6;font-weight:500;font-family:monospace;font-size:10px;letter-spacing:0.1em">DETAIL</th>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04)">
<td style="padding:9px 14px;color:#8A94A6;font-size:12px">Language</td>
<td style="padding:9px 14px;color:#B0B8C8">Python 3</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04);background:rgba(255,255,255,0.02)">
<td style="padding:9px 14px;color:#8A94A6;font-size:12px">Regression</td>
<td style="padding:9px 14px;color:#B0B8C8">statsmodels Logit — for interpretable coefficients and p-values</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04)">
<td style="padding:9px 14px;color:#8A94A6;font-size:12px">Evaluation</td>
<td style="padding:9px 14px;color:#B0B8C8">scikit-learn — confusion matrix, ROC-AUC, classification report</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04);background:rgba(255,255,255,0.02)">
<td style="padding:9px 14px;color:#8A94A6;font-size:12px">Data handling</td>
<td style="padding:9px 14px;color:#B0B8C8">pandas, numpy</td>
</tr>
<tr style="border-bottom:1px solid rgba(255,255,255,0.04)">
<td style="padding:9px 14px;color:#8A94A6;font-size:12px">Visualisation</td>
<td style="padding:9px 14px;color:#B0B8C8">matplotlib, seaborn</td>
</tr>
<tr>
<td style="padding:9px 14px;color:#8A94A6;font-size:12px">Dataset</td>
<td style="padding:9px 14px;color:#B0B8C8">Portuguese Bank Marketing — UCI ML Repository (Moro et al., 2014)</td>
</tr>
</table>

<br/>

---

<!-- FOOTER -->
<div align="center">
<br/>
<table cellspacing="0" cellpadding="0" style="background:#0D1E35;border:1px solid rgba(201,168,76,0.2);max-width:560px;width:100%">
<tr>
<td style="padding:20px 28px">
<p style="margin:0 0 4px 0;font-size:15px;font-weight:700;color:#FFFFFF">Sana Majeed</p>
<p style="margin:0 0 12px 0;font-size:12px;color:#8A94A6">MS Business Analytics · Purdue University</p>
<p style="margin:0;font-size:12px;color:#8A94A6">
<a href="https://linkedin.com/in/sanamjumani" style="color:#C9A84C;text-decoration:none">LinkedIn</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/sanamjummani" style="color:#C9A84C;text-decoration:none">GitHub</a>
</p>
</td>
</tr>
</table>
<br/>
<p style="font-size:11px;color:#4A5568;font-style:italic">Part of a portfolio of data-driven strategy projects built during the MS BAIM program at Purdue.</p>
<br/>
</div>
