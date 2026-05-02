# Perplexity Signal — Micron NLP Stock Pitch

A single-page case study applying NLP perplexity signals to Micron Technology earnings call transcripts. April 2026.

The site is fully static — plain HTML, two CSS files, three chart images, and the two source PDFs. No build step required.

## Project Structure

```
.
├── index.html                                      # Main case study page
├── base.css                                        # CSS reset + base styles
├── style.css                                       # Theme tokens + components
├── assets/
│   ├── chart1.png                                  # Cumulative L/S returns
│   ├── chart2.png                                  # Quintile distributions
│   └── chart3.png                                  # Perplexity vs. return scatter
├── Micron Technology Equity Research Memo.pdf      # Full equity memo (linked)
├── Mircon Technology NLP Analysis.pdf              # NLP methodology (linked)
├── .nojekyll                                       # Tells GitHub Pages not to run Jekyll
└── README.md                                       # This file
```
