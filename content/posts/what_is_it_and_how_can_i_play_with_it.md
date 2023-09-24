---
title: "What is this and how can I play with it"
date: 2023-09-24
categories: [communication]
draft: true
---

When writing about a new feature, product, etc. the first two questions I want answered before anything else are **what is it?** and **how can I play with it?**.
I first encountered this construction in one (or both?) of two books I had as a child, [Explorabook](https://www.goodreads.com/en/book/show/558728) and [Earthsearch](https://www.goodreads.com/book/show/370703.Earthsearch).

## What is it?
- One to two sentences, bolded.
- Written for a general audience, and appears "above the fold"
- Readers immediately can judge whether they care about your thing, and pass on it if not

## How do I play with it?
- Immediate call to action
- Lets a curious reader jump right in before having to read a bunch of context
- Allows for a curious audience to get a real feel for the capabilities of the thing, not just read about it
- _Proves usefulness_.  This section is a good bellwether for whether the thing is actually useful.  If you can't demonstrate usefulness, maybe it isn't actually useful. 
- _Actually works_.  This section can be sample code, a link to a demo or a quickstart guide, but importantly you need to make sure it actually works.

## Example

### What is it?
**We've launched a new data model `domain.daily_summary`, containing daily rollups of metric X by entity Y and bucketed attributes.**

### How do I play with it?
```sql
SELECT
  date,
  SUM(metric_x) AS total_metric_x
FROM
  domain.daily_summary
WHERE
  entity_y_id IN (1, 2, 3)
GROUP BY 1
```

Click [here] to open a sample query!

### More context

- Important context 1
- ...

## So what?
When I'm announcing something at work, I will paste in these two questions as draft headings before starting to write.
The headings may change, and there may be more content afterwards, but I try to make sure the audience can answer these two questions within the first paragraph. 