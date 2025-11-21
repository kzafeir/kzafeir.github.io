---
title: "Adjusting Product Representations for Sequential Recommender Systems"
collection: posters
type: "Poster Presentation"
permalink: /posters/2025-06-adjusting-product-representations
venue: "MSc AI Research Showcase, Lab42"
date: 2025-06-01
location: "University of Amsterdam, Amsterdam, The Netherlands"
posterurl: '/files/poster-RCS.pdf'
excerpt: 'Reproduced Recformer across Amazon and MIND benchmarks, compared it to ID-only, hybrid, and text-first baselines, and tested an ABSA extension to study accuracy, fairness, and cross-domain diversity.'
---

## Abstract

This poster reports on reproducing Recformer, a text-first sequential recommender that replaces item IDs with detailed product descriptions, and benchmarking it against ID-only (SASRec), hybrid (FDSA), and text-only (UniSRec) models. We target two large-scale datasets—Amazon Reviews and Microsoft MIND—to understand how product representations influence accuracy, generalization, and diversity. Beyond reproduction, we extend Recformer with aspect-based sentiment annotations derived from user reviews (<em>Recformer-ABSA</em>) to evaluate whether richer textual cues improve sequential next-item prediction.

## Methodology

- Follow the published Recformer training recipe with minor adjustments for available hardware.
- Pre-train each model on multiple product/news categories and fine-tune on two specific categories per dataset.
- Evaluate accuracy (NDCG, Recall, MRR) together with diversity and fairness metrics (Gini, Intra-List Diversity, Catalog Coverage).
- Append aspect-based sentiment triplets extracted via a BERT-based ABSA model to product titles for the Recformer-ABSA variant.

## Key Findings

- Recformer replicates the original in-domain performance trends on Amazon and generally outperforms ID-based baselines when product text is available.
- Cross-domain transfer from Amazon to MIND remains challenging for every approach; Recformer’s advantage narrows substantially on news content.
- Diversity analysis reveals Recformer produces globally balanced catalogs (low Gini) yet lower intra-list diversity, while UniSRec shows the opposite trade-off.
- Injecting sentiment-aware aspects did not boost metrics, suggesting that naïvely concatenating ABSA features can introduce noise without richer modeling.

## Team

**Jonas Schoonhoven**, **Konstantinos Zafeirakis**, **Luc Buijs**, **Coen Giezen**

## Download

[Download Poster PDF](/files/poster-RCS.pdf)

