# TensorFlow demo

**Demo — small Keras net predicts car fuel efficiency (MPG).**

Not a client case study. A compact walkthrough of tabular regression with TensorFlow/Keras: clean data, scale, train a 3-layer net, read the loss curve.

---

## What it shows

| Step | What happens |
|------|----------------|
| Data | Auto MPG (~400 cars) — cylinders, power, weight, year, origin |
| Clean | Impute a few missing horsepower values |
| Encode | Origin → one-hot |
| Scale | Standardise features + target |
| Model | Dense 32 → 64 → 1 · RMSProp · MSE |
| Read | Train/val loss · predictions in real MPG units |

## When to use it

- Learning **Keras on tabular data**  
- Teaching **scale / encode / inverse-transform**  
- Baseline before more exotic models  

## When not to

- Business ROI stories — see the case studies on my profile  
- Large production systems  

## Run it

```bash
pip install tensorflow pandas scikit-learn matplotlib
git clone https://github.com/47096/tensorflow-demo.git
cd tensorflow-demo
jupyter notebook analysis.ipynb
```

**Data:** `data/auto-mpg.data` (UCI Auto MPG, vendored)

**Stack:** TensorFlow/Keras · pandas · scikit-learn · matplotlib

---

*Demo companion — [datafying](https://datafying.co/) case studies live in the pinned repos.*
