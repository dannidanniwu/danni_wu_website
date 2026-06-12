---
title: "Hello, world (with a prior)"
date: 2026-06-11
tags: [meta]
---

Welcome to my blog! I plan to use this space for notes on Bayesian statistics, clinical trial design, and statistical computing in R — the kind of things that don't quite fit in a paper but are too useful to keep in a drawer.

## How this blog works

This site is built with Jekyll on GitHub Pages, so writing a new post is just adding a Markdown file to the `_posts` folder, named like `2026-06-11-my-post-title.md`, with a small header at the top:

```yaml
---
title: "My post title"
date: 2026-06-11
tags: [bayesian, R]
---
```

Everything below the header is plain Markdown. Code blocks render nicely too:

```r
library(rstan)

# A minimal Beta-Binomial update
prior_a <- 1; prior_b <- 1
successes <- 7; trials <- 10

posterior <- rbeta(1e4, prior_a + successes, prior_b + trials - successes)
quantile(posterior, c(0.025, 0.5, 0.975))
```

More soon.
