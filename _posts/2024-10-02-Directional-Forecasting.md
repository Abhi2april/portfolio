---
description: Predicting weather the crypto prices will surge or not, for the next minute using the o.h.l.c.v. data features.
title: Directional Forecastion
toc: true
badges: true
comments: true
author: Abhishek Singh
categories: [Random Forest, Scikit Learn]
image: images/posts/rag.png
cover: images/covers/rag.png
layout: notebook
permalink: /blog/:year:month:day/Directional-Forecasting
sticky_rank: 2
---

<p>This post was originally published on my <a href="https://github.com/Abhi2april/Directional-Forecasting/blob/main/crypto_main.ipynb">github_repository</a></p>

<h1 id="1.-Introduction">1. Introduction<a class="anchor-link" href="#1.-Introduction"> </a>
<p>This post consists of, how basic machine learning and python libraries can be tailored for most of Finance Data Science like in here we are using Random Forest for directional forecasting of a cryptocurrency data consisting of features 'open', 'high', 'low', 'close', 'volume', 'taker_buy_volume_ratio' etc.. with their given 'timestamp's'(useful for extracting month, day, date, hour, minutes) of minutes' basis, containing 2.1 million rows.</p>
<!--
<h1 id="2.-Full Post">2. Full Post<a class="anchor-link" href="#2.-Full Post"> </a>
<p>... <a href="https://aws.amazon.com/blogs/machine-learning/improve-llm-responses-in-rag-use-cases-by-interacting-with-the-user/"> (continue reading here)</a></p>
