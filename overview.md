---
layout: default
title: Algorithm Overview
nav_order: 2
permalink: /overview
---

# Algorithm Overview
{: .no_toc }

Read the summaries below to determine which of our matching algorithms is right for you.
{: .fs-6 .fw-300 }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Dynamic Almost Matching Exactly (DAME)

<table class="overview">
  <tr>
    <td><b>Languages</b>:</td> 
    <td>Python</td>
  </tr>
  <tr>
    <td><b>Input data</b>:</td>
    <td>Categorical covariates, works best with small to moderately-sized datasets</td>
  </tr>
  <tr>
    <td><b>Matching method</b>:</td>
    <td>Uses bit-vector computations to match units based on a learned, weighted Hamming 
    distance.</td>
  </tr>
  <tr>
    <td><b>Paper</b>:</td>
    <td><a>Interpretable Almost Matching Exactly for Causal Inference</a></td>
  </tr>
</table>

## Fast Large-Scale Almost Matching Exactly (FLAME)

<table class="overview">
  <tr>
    <td><b>Languages</b>:</td> 
    <td>R, Python</td>
  </tr>
  <tr>
    <td><b>Input data</b>:</td>
    <td>Categorical covariates, scales well to large datasets with millions of observations</td>
  </tr>
  <tr>
    <td><b>Matching method</b>:</td>
    <td>Uses bit-vector computations to match units based on a learned, weighted Hamming distance. 
    FLAME successively drops irrelevant covariates to lessen the computational load while still 
    maintaining enough covariates for high-quality conditional average treatment effect (CATE) 
    estimation.</td>
  </tr>
  <tr>
    <td><b>Paper</b>:</td>
    <td><a>FLAME: A Fast Large-scale Almost Matching Exactly Approach to Causal Inference</a></td>
  </tr>
</table>

## Matching After Learning to Stretch (MALTS)

<table class="overview">
  <tr>
    <td><b>Languages</b>:</td> 
    <td>Python</td>
  </tr>
  <tr>
    <td><b>Input data</b>:</td>
    <td>Continuous, categorical, or mixed (continous and categorical) covariates</td>
  </tr>
  <tr>
    <td><b>Matching method</b>:</td>
    <td>Uses exact matching for discrete variables and learned, generalized Mahalanobis distances 
    for continuous variables. Instead of a predetermined distance metric, the covariates 
    contributing more towards predicting the outcome are given higher weights.</td>
  </tr>
  <tr>
    <td><b>Paper</b>:</td>
    <td><a>Matching After Learning To Stretch</a></td>
  </tr>
</table>

## Adaptive Hyper-Box Matching (AHB)

<table class="overview">
  <tr>
    <td><b>Languages</b>:</td> 
    <td>R</td>
  </tr>
  <tr>
    <td><b>Input data</b>:</td>
    <td>Continuous, categorical, or mixed (continous and categorical) covariates</td>
  </tr>
  <tr>
    <td><b>Matching method</b>:</td>
    <td>Matches units with others in unit-specific, hyper-box-shaped regions of the covariate space. 
    The regions are found as either the solution to a mixed integer program, or by using a fast 
    approximation algorithm.</td>
  </tr>
  <tr>
    <td><b>Paper</b>:</td>
    <td><a>	Adaptive Hyper-box Matching for Interpretable Individualized Treatment Effect 
    Estimation</a></td>
  </tr>
</table>
