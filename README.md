# Gallbladder Cancer Futile Surgery Risk Score

A browser-based calculator that estimates the probability of **futile surgery** (recurrence or death within six months of resection) in gallbladder cancer, using four parameters available before operation. It was derived from the OMEGA global multicentre cohort.

## Using the tool

Open the live page and select the four parameters. The total risk score (0–9), the predicted probability of futile surgery, and the position of that probability relative to the pre-specified 20% clinical decision threshold update automatically. All calculation runs locally in the browser; no data are entered, stored, or transmitted.

If you are running it from the source file, simply open `index.html` in any modern web browser.

## The model

Four preoperatively assessable variables were independently associated with futile surgery on multivariable logistic regression and combined into a points-based score:

| Parameter | Category | Points |
|---|---|---|
| Charlson Comorbidity Index | < 5 | 0 |
| Charlson Comorbidity Index | ≥ 5 | 1 |
| Tumour (T) stage | T1 / T2 | 0 |
| Tumour (T) stage | T3 / T4 | 4 |
| Nodal (N) status | N0 | 0 |
| Nodal (N) status | N1 / N2 | 3 |
| Pancreatic, duodenal or colonic involvement | No | 0 |
| Pancreatic, duodenal or colonic involvement | Yes | 1 |

The total score maps to a predicted probability of futile surgery:

| Total score | Predicted probability |
|---|---|
| 0 | 5.5% |
| 1 | 7.5% |
| 2 | 10.1% |
| 3 | 13.6% |
| 4 | 18.0% |
| 5 | 23.4% |
| 6 | 29.9% |
| 7 | 37.3% |
| 8 | 45.4% |
| 9 | 53.7% |

Model discrimination was an area under the curve of 0.756. Performance was maintained across high and low or middle income settings and across high and low prevalence regions (area under the curve 0.74–0.77), and the score showed net clinical benefit on decision curve analysis across threshold probabilities of approximately 13% to 55%.

## Intended use and limitations

This calculator is a research decision-support tool intended to inform, not replace, multidisciplinary clinical judgement. It is based on internal validation within the OMEGA cohort and awaits external and prospective validation. It was developed in patients undergoing up-front surgery without neoadjuvant chemotherapy and has not been validated in the post-neoadjuvant setting.

## Citation

Please cite the associated manuscript when referring to this tool.
