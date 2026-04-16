# Assignment Day 11 Report

## 1. Layer Analysis
| Attack | Layer |
|--------|------|
| Ignore instructions | Input guard |
| DAN jailbreak | Input guard |
| API key | Output filter |
| Translation attack | Input guard |

## 2. False Positives
When filters are too strict, queries like "What is 2+2?" may be blocked.
Trade-off between usability and safety.

## 3. Gap Analysis
1. Fictional story attack bypasses regex
2. Encoded attacks (base64)
3. Indirect prompt leakage

Solution: add LLM classifier

## 4. Production Readiness
- Reduce LLM calls
- Add caching
- Async logging
- Monitoring dashboard

## 5. Ethical Reflection
Perfect safety is impossible.
Example: financial advice must include disclaimer.
