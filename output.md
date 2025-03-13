# Output 2025/03/13
```
zyz23@zyz-4080s:~/project/ai-financial-agent$ poetry run python src/main.py --ticker TSLA,NVDA
? Select your AI analysts. done (10 selections)

Selected analysts: Ben Graham, Bill Ackman, Cathie Wood, Charlie Munger, Stanley Druckenmiller, Warren Buffett, Technical Analyst, Fundamentals Analyst, Sentiment Analyst, Valuation Analyst

? Select your LLM model: [deepseek] deepseek-r1

Selected DeepSeek model: deepseek-reasoner

 ✓ Ben Graham          [NVDA] Done                                                                    
 ✓ Bill Ackman         [NVDA] Done                                                                    
 ✓ Cathie Wood         [NVDA] Done                                                                    
 ✓ Charlie Munger      [NVDA] Done                                                                    
 ✓ Fundamentals        [NVDA] Done                                                                    
 ✓ Sentiment           [NVDA] Done                                                                    
 ✓ Stanley Druckenmiller[NVDA] Done                                                                   
 ✓ Technical Analyst   [NVDA] Done                                                                    
 ✓ Valuation           [NVDA] Done                                                                    
 ✓ Warren Buffett      [NVDA] Done                                                                    
 ✓ Risk Management     [NVDA] Done                                                                    
 ✓ Portfolio Management[NVDA] Done                                                                    

Analysis for TSLA
==================================================

ANALYST SIGNALS: [TSLA]
+-----------------------+----------+--------------+
| Analyst               |  Signal  |   Confidence |
+=======================+==========+==============+
| Fundamentals          | BEARISH  |        50.0% |
+-----------------------+----------+--------------+
| Valuation             | BEARISH  |        99.0% |
+-----------------------+----------+--------------+
| Technical Analyst     | BEARISH  |          28% |
+-----------------------+----------+--------------+
| Sentiment             | BEARISH  |        76.0% |
+-----------------------+----------+--------------+
| Ben Graham            | BEARISH  |        95.0% |
+-----------------------+----------+--------------+
| Cathie Wood           | BEARISH  |        68.5% |
+-----------------------+----------+--------------+
| Stanley Druckenmiller | NEUTRAL  |        45.0% |
+-----------------------+----------+--------------+
| Warren Buffett        | BEARISH  |        90.5% |
+-----------------------+----------+--------------+
| Charlie Munger        | BEARISH  |        72.5% |
+-----------------------+----------+--------------+
| Bill Ackman           | BEARISH  |        85.2% |
+-----------------------+----------+--------------+
| Risk Management       |          |        None% |
+-----------------------+----------+--------------+

TRADING DECISION: [TSLA]
+------------+-------+
| Action     | SHORT |
+------------+-------+
| Quantity   |    80 |
+------------+-------+
| Confidence | 73.9% |
+------------+-------+

Reasoning: Strong bearish consensus from 9/10 agents with average confidence 73.86%. Max shares shorted within margin and position limits.

Analysis for NVDA
==================================================

ANALYST SIGNALS: [NVDA]
+-----------------------+----------+--------------+
| Analyst               |  Signal  |   Confidence |
+=======================+==========+==============+
| Fundamentals          | BULLISH  |       100.0% |
+-----------------------+----------+--------------+
| Valuation             | BEARISH  |        75.0% |
+-----------------------+----------+--------------+
| Technical Analyst     | BEARISH  |          23% |
+-----------------------+----------+--------------+
| Sentiment             | BEARISH  |        74.0% |
+-----------------------+----------+--------------+
| Ben Graham            | NEUTRAL  |        45.0% |
+-----------------------+----------+--------------+
| Cathie Wood           | BULLISH  |        65.0% |
+-----------------------+----------+--------------+
| Stanley Druckenmiller | NEUTRAL  |        55.0% |
+-----------------------+----------+--------------+
| Warren Buffett        | BEARISH  |        75.0% |
+-----------------------+----------+--------------+
| Charlie Munger        | NEUTRAL  |        65.0% |
+-----------------------+----------+--------------+
| Bill Ackman           | NEUTRAL  |        35.0% |
+-----------------------+----------+--------------+
| Risk Management       |          |        None% |
+-----------------------+----------+--------------+

TRADING DECISION: [NVDA]
+------------+-------+
| Action     |  HOLD |
+------------+-------+
| Quantity   |     0 |
+------------+-------+
| Confidence | 61.2% |
+------------+-------+

Reasoning: Conflicting signals: bullish fundamentals (100% confidence) vs. bearish valuation (75%), sentiment (74%), and Warren Buffett (75%). Average confidence 61.2% indicates no clear direction.

PORTFOLIO SUMMARY:
+----------+----------+------------+--------------+
| Ticker   |  Action  |   Quantity |   Confidence |
+==========+==========+============+==============+
| TSLA     |  SHORT   |         80 |        73.9% |
+----------+----------+------------+--------------+
| NVDA     |   HOLD   |          0 |        61.2% |
+----------+----------+------------+--------------+

```