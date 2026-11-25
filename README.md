# Maketo Bitcoin Fear & Greed Index, Daily History

Maketo's daily Bitcoin market-mood reading from 0 (extreme fear) to 100 (extreme greed), since 1 Jan 2016.

**This copy ends on 31 Oct 2026.** Today's reading, and what is driving it, is on the live page:
**[Maketo Fear & Greed](https://maketo.com/fear-greed)** at maketo.com, updated once a day.

## File

`maketo_fear_greed_daily.csv`: 3,953 rows, one per UTC day.

| Column | Meaning |
|---|---|
| `date` | The UTC day, as YYYY-MM-DD. |
| `value` | The reading, from 0 (extreme fear) to 100 (extreme greed). |
| `zone` | Under 15 extreme fear, 15 to 34 fear, 35 to 55 neutral, 56 to 74 greed, 75 or more extreme greed. |
| `parts_used` | How many of the six parts had data that day (see below). |
| `worked_out_later` | `yes` if the reading was worked out afterwards, `no` if it was recorded on the day. |
| `method_version` | The version of the method used for that day. |
| `source_url` | The Maketo page with the live reading and its history. |

## What the reading is

Maketo's Fear & Greed reading blends six parts of the market: what holders are doing on the blockchain, money
flowing into Bitcoin funds, the tone of the news, how the price is moving, how miners are faring, and how much the
public searches for Bitcoin. Each part is scored from 0 to 100, then weighted into one number, rebuilt every day.
It describes the market's mood. It is not a forecast of the price and not advice to buy or sell.

This is Maketo's own index. It is not the same series as other fear and greed indexes, which use different inputs.

From 30 May 2026 each reading was recorded on its own day. Readings before 30 May 2026 were worked out afterwards with the same method, so today can be compared with the past (`worked_out_later` = `yes`). They are context, not proof that anyone could have traded on them at the time. Before 11 Jan 2024 only three parts (holders, price and miners) have records that go back that far,
which is why `parts_used` is lower on older days. No reading was recorded on 22 to 25 Oct 2026; those days have no row, and the live page shows the last reading before a missing day. The full method is at
[maketo.com/fear-greed/methodology](https://maketo.com/fear-greed/methodology).

## Licence and credit

CC BY 4.0 ([https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)). You may copy, share and build on this data, including for commercial use,
as long as you credit Maketo with a link. Suggested credit:

> Source: Maketo Fear & Greed Index, https://maketo.com/fear-greed

## Updates

A new copy is published at the start of each month, ending on the last day of the month before.
The same data is on GitHub ([Maketocom/maketo-fear-greed-index](https://github.com/Maketocom/maketo-fear-greed-index)),
Hugging Face ([Maketocom/maketo-fear-greed-index](https://huggingface.co/datasets/Maketocom/maketo-fear-greed-index))
and Kaggle ([maketocom/maketo-fear-greed-index](https://www.kaggle.com/datasets/maketocom/maketo-fear-greed-index)).

## Permanent copy (DOI)

Every three months a copy is archived at Zenodo, under one permanent DOI: [10.5281/zenodo.24523489](https://doi.org/10.5281/zenodo.24523489). Researchers can cite that DOI; it always leads to the latest version.

This data is for learning and research. It is not financial advice.
