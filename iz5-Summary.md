---
layout: page
title: Summary
permalink: /Summary/
---


We learn that
1. representing data is always an open question. You need to fully explore the data than you can find the right way to do it.
2. Choosing models is not originally important, we can train them all and compare. But models typically will give reasonable result as you originally explore. Therefore, process to choose model will increase your efficiency
3. For ill-conditioned problems, fit another model to make the problem more regular might not improve the result (sequential modeling might introducing too much variation). But use some exploration result from the data to make the problem less ill-conditioned can help, which suggest us to fully explore the data before modeling and not using modeling itself to assist modeling.

We justify our answers through a randomly assigned test dataset

The limitatiion is that actually the dataset encode a lot of the web behavior and some of the features are happening across the visiting process, therefore some of the features may not be observed at the begining stage. Therefore as a pure prediction model, the useful case of this might be limited.
