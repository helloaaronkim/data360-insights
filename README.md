# Data 360 Demo Collection

Interactive demo files for Salesforce Data 360 training and presentations.  
Salesforce Data 360 トレーニング・プレゼンテーション用インタラクティブデモ集。

---

## Files / ファイル一覧

| File | Language | Description |
|------|----------|-------------|
| `data360-timeline.html` | 한국어 | Customer Journey Timeline — 12 Korean customers, 94 events |
| `data360-timeline-ja.html` | 日本語 | Customer Journey Timeline — 日本人顧客12名、94イベント |
| `streaming-insights-demo.html` | 한국어 | Streaming Insights real-time event simulation |
| `streaming-insights-ja.html` | 日本語 | Streaming Insights リアルタイムイベントシミュレーション |

No server or deployment required. Open any `.html` file directly in a browser.  
サーバー不要。`.html` ファイルをブラウザで直接開くだけで動作します。

---

## Customer Journey Timeline

**Concepts covered / 学習ポイント**

- Unified Individual DMO — single unified profile across all sources
- Data Streams — Web, App, CRM, Email, Offline channel integration
- Identity Resolution — cross-channel customer matching
- Einstein Next Best Action — personalized recommendation display
- Source filtering and month-grouped timeline view

**How to use / 使い方**

1. Open the HTML file in a browser
2. Select a customer from the left sidebar
3. Use source filter buttons to narrow the timeline by channel
4. Use segment pills (High Value / Loyal / At-Risk / New / Regular) to filter the list

---

## Streaming Insights

**Concepts covered / 学習ポイント**

- Streaming Insights SQL syntax — `WITHIN`, `HAVING`, time window aggregation
- Real-time event evaluation against defined insight rules
- Cross-source JOIN (App + Offline) for omnichannel behavior detection
- Action triggers — Flow, Email Campaign, SMS, Profile Update, CS Alert

**Active insights / アクティブInsight一覧**

| Insight | Condition | Action |
|---------|-----------|--------|
| High Purchase Intent | 3+ page views within 5 min | Personalized offer popup (Flow) |
| Cart Abandonment Risk | add_to_cart → checkout_abandon | Win-back email + 10% coupon |
| Purchase Conversion | purchase event detected | Thank-you SMS + reward points |
| Cross-Channel Behavior | app_open → store_visit within 60 min | Unified Profile update |
| Churn Signal | 2+ remove_from_cart within 2 min | CS alert + 15% discount coupon |

**How to use / 使い方**

1. Open the HTML file in a browser
2. Click **▶ Start** (or **▶ ストリーミング開始**) to begin the event stream
3. Watch the center panel — condition progress bars fill in real time
4. When a rule fires, the card flashes and the action appears in the right panel
5. Use the speed selector to control the event generation rate

---

## Classroom Talking Points

**Data 360 Timeline**
> "In real Data 360, these custom objects are created automatically from connected data streams. Identity Resolution merges records from different sources into a single Unified Individual — what you see here as one profile."

**Streaming Insights**
> "This SQL runs continuously against incoming streaming data — not against stored records. The `WITHIN 5 MINUTES` clause defines a rolling time window. When the `HAVING` condition is met, the insight fires and triggers an action immediately, without any scheduled batch process."

---

*All data is fictional and for demonstration purposes only.*  
*すべてのデータはデモ用の架空データです。*
