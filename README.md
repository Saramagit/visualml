# The Visual ML Explainer

An interactive lab for seven foundational machine-learning methods. Drag the data, move the sliders, watch the models change.

![Preview](<img width="800" height="468" alt="preview" src="https://github.com/user-attachments/assets/dcbb6759-60ed-411d-97a9-ce82bd452f43" />
)

**Live site:** [saramagit.github.io/visualml](https://saramagit.github.io/visualml/)

## What's inside

Seven classical classifiers, each with its own interactive playground:

| Method | What it shows |
|---|---|
| **Linear / Logistic** | The line that splits the plane, and why straight boundaries can't wrap a ring |
| **Decision Trees** | Axis-aligned splits, readable as a flowchart |
| **k-Nearest Neighbors** | Voronoi-like neighborhoods; effect of `k` on smoothness |
| **Support Vector Machine** | Margin maximization; linear vs RBF kernel |
| **Naive Bayes** | Probability fields from a "naive" independence assumption |
| **Neural Network** | How a tiny MLP bends the boundary with ReLU units |
| **Random Forest** | Ensemble voting turning wobbly trees into a smooth surface |

Plus a dedicated **Evaluation** section covering the score-distribution view, ROC / AUC, threshold sweep, confusion matrix, and precision vs recall tradeoffs — all driven by a live classifier you can make better or worse with a slider.

## Use it in a classroom

Every view has a **Scenario** mode that grounds the abstract math in a named, stakes-aware setup (mortgage underwriting, ER triage, fraud, handwritten-digit routing, and so on). Each scenario spells out what a false positive and false negative cost, so students can argue about which error the model should minimize.

Switch to **Lab** mode for the raw math view when that's what you want.

## Run locally

It's a single HTML file, no build step, no server required.

```bash
git clone https://github.com/saramagit/mlexplainer.git
cd mlexplainer
open index.html    # or just double-click it
```

## Tech

Hand-written React (loaded via CDN, no bundler) with `<canvas>` rendering for every classifier. The entire site, including all fonts, is packaged into one self-contained HTML file that works offline.

## License

MIT
