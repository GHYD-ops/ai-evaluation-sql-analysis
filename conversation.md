# Conversation Transcript

**Project type:** Self-directed bilingual business-analysis simulation  
**Business:** Fictional Saudi online gift store  
**Data type:** Synthetic training data

**Editorial note:** This transcript is a revised learning simulation, not a real customer exchange. Its reported sales figures can be checked against the linked SQL dataset; operational explanations are fictional scenario statements, not independently verified findings.

## 1. Scenario Exploration

### Analyst - Saudi Arabic

وش أبرز التغيرات في المبيعات خلال آخر شهرين؟ عطيني الأرقام حسب المنتج والمدينة وقناة البيع.

### Business Stakeholder

بحسب آخر شهرين مكتملين، ارتفع إجمالي المبيعات من **420,000 ريال في أغسطس** إلى **505,000 ريال في سبتمبر**، وارتفع عدد الطلبات من **1,240 إلى 1,430**.

**حسب المنتج - المبيعات بالريال**

| المنتج | أغسطس | سبتمبر |
|---|---:|---:|
| الزهور | 105,000 | 125,000 |
| الشوكولاتة | 80,000 | 93,000 |
| الهدايا المخصصة | 92,000 | 118,000 |
| العطور | 76,000 | 84,000 |
| هدايا الشركات | 67,000 | 85,000 |

**حسب المدينة**

| المدينة | أغسطس | سبتمبر |
|---|---:|---:|
| الرياض | 190,000 | 230,000 |
| جدة | 112,000 | 130,000 |
| الدمام | 75,000 | 87,000 |
| أبها | 43,000 | 58,000 |

**حسب قناة البيع**

| القناة | أغسطس | سبتمبر |
|---|---:|---:|
| الموقع الإلكتروني | 210,000 | 247,000 |
| إنستغرام وواتساب | 125,000 | 150,000 |
| منصات البيع الخارجية | 55,000 | 62,000 |
| مبيعات الشركات المباشرة | 30,000 | 46,000 |

وش تحب نحلل أول: المنتجات، المدن، أو قنوات البيع؟

## 2. Monthly Performance

### Analyst - Saudi Arabic

كم إجمالي المبيعات وعدد الطلبات في كل شهر؟

### Business Stakeholder

| الشهر | إجمالي المبيعات | عدد الطلبات |
|---|---:|---:|
| أغسطس | 420,000 ريال | 1,240 |
| سبتمبر | 505,000 ريال | 1,430 |

عمليًا، سبتمبر أعلى من أغسطس في المبيعات وعدد الطلبات.

## 3. Product Performance

### Analyst - Saudi Arabic

وش المنتجات الأعلى مبيعًا والأقل؟ وهل تغير ترتيبها؟

### Business Stakeholder

بالاعتماد على قيمة المبيعات:

- الأعلى مبيعًا: الزهور في الشهرين؛ 105,000 ريال في أغسطس و125,000 ريال في سبتمبر.
- الثاني: الهدايا المخصصة.
- الأقل في أغسطس: هدايا الشركات، بقيمة 67,000 ريال.
- الأقل في سبتمبر: العطور، بقيمة 84,000 ريال.

نعم، تغير الترتيب في المركزين الأخيرين: هدايا الشركات تقدمت على العطور في سبتمبر.

## 4. City Performance

### Analyst - Saudi Arabic

كيف تختلف المبيعات بين الرياض وجدة والطائف؟

### Business Stakeholder

حسب التقرير الحالي:

| المدينة | أغسطس | سبتمبر |
|---|---:|---:|
| الرياض | 190,000 ريال | 230,000 ريال |
| جدة | 112,000 ريال | 130,000 ريال |
| الطائف | غير متاحة في التقرير | غير متاحة في التقرير |

الرياض هي الأعلى بوضوح، تليها جدة. والطائف ليست ضمن المدن التي نتابعها بشكل منفصل حاليًا.

## 5. Sales Channel Performance

### Analyst - Saudi Arabic

هل إيرادات إنستغرام أعلى من الموقع؟ عطيني مقارنة بالأرقام.

### Business Stakeholder

ما نقدر نقارن إنستغرام وحده بالموقع؛ لأن التقرير يجمع مبيعات **إنستغرام وواتساب في قناة واحدة**. لكن نقدر نقارن قيمة إيرادات الموقع بهذه القناة المجمّعة:

| القناة | أغسطس | سبتمبر |
|---|---:|---:|
| الموقع الإلكتروني | 210,000 ريال | 247,000 ريال |
| إنستغرام وواتساب | 125,000 ريال | 150,000 ريال |

إيرادات الموقع أعلى من القناة المجمعة بـ85,000 ريال في أغسطس و97,000 ريال في سبتمبر. هذا لا يثبت أن معدل التحويل أو الربحية أفضل؛ نحتاج بيانات الزيارات والتكاليف لكل قناة.

## 6. Customer Behavior

### Analyst - Saudi Arabic

هل الانخفاض في عدد العملاء الجدد أو العملاء المتكررين؟

### Business Stakeholder

الانخفاض كان في العملاء المتكررين، وليس الجدد:

| نوع العميل | أغسطس | سبتمبر |
|---|---:|---:|
| عملاء جدد | 780 | 910 |
| عملاء متكررون | 430 | 410 |

فالعملاء الجدد زادوا، بينما العملاء المتكررون انخفضوا قليلًا.

## 7. Average Order Value

### Analyst - Saudi Arabic

هل تغير متوسط قيمة الطلب خلال الفترة؟

### Business Stakeholder

نعم، ارتفع متوسط قيمة الطلب:

| الشهر | متوسط قيمة الطلب |
|---|---:|
| أغسطس | 339 ريال تقريبًا |
| سبتمبر | 353 ريال تقريبًا |

أي بزيادة تقارب 14 ريالًا للطلب الواحد، أو حوالي 4%.

## 8. Operations and Promotions

### Analyst - English

Were there any changes in pricing, promotions, stock availability, or delivery times?

### Business Stakeholder

Yes, there were several changes in September:

- Pricing: Base prices stayed mostly unchanged, but average discounts increased from about 8% to 11%.
- Promotions: We offered free delivery on orders above 250 SAR and a promotion on personalized gifts.
- Stock: Some perfume items were unavailable for about a week. Personalized-gift materials were also temporarily limited.
- Delivery times: Riyadh and Jeddah stayed around 1-2 days. Abha increased from roughly 2.5 to 3.5 days due to courier capacity.

## 9. Customer Complaints

### Analyst - English

What are the most common customer complaints during this period?

### Business Stakeholder

The most common complaints in August and September were:

| Complaint type | Cases | Share |
|---|---:|---:|
| Late delivery | 62 | 33% |
| Product looked different from photos | 38 | 20% |
| Personalization errors | 31 | 17% |
| Damaged packaging | 24 | 13% |
| Out-of-stock items or cancellations | 18 | 10% |
| Wrong item or delivery address | 13 | 7% |

These complaint counts cover both months together. They cannot show whether late deliveries became more frequent in September or in Abha. The separate scenario notes longer delivery times to Abha in September, but this table cannot validate that claim.

## 10. Data Needed for a Final Conclusion

### Analyst - English

What additional data would you need before making a final conclusion?

### Business Stakeholder

Before making a final conclusion, I would need:

- Profit margin by product, city, and channel, not just sales revenue.
- Discount and promotion details, including whether promotions created incremental sales.
- Customer cohorts, showing repeat purchases over 30, 60, and 90 days.
- Stock-out records by product and date.
- Delivery performance by city, courier, and promised versus actual delivery time.
- Cancellation, return, and refund rates by product and channel.
- Marketing cost and customer acquisition cost for each channel.
- Complaint rates per order, so high-volume channels are compared fairly.

Without this data, we can identify patterns, but not confidently determine the main business cause.

## 11. Leading Hypothesis

### Analyst - English

Based on the available information, which possible cause seems most likely?

### Business Stakeholder

A possible explanation is that promotions coincided with higher sales while operational friction may have affected repeat purchasing.

The data shows higher revenue, more orders, a higher average order value, and fewer reported repeat customers. The simulated stakeholder also reports increased discounts and some fulfillment constraints. However, the complaints dataset has no month or city identifiers, so it cannot establish whether complaints increased or whether these issues caused the change in repeat-customer counts. Profitability and cohort retention are not measured.

This remains a hypothesis, not a confirmed causal conclusion.

## 12. Recommended Priority

### Analyst - English

What should the store prioritize first, and why?

### Business Stakeholder

I would prioritize delivery reliability and stock availability first.

Late delivery accounts for 62 of 186 complaints (33.33%) across the two months. Repeat-customer counts fell from 430 to 410, and the simulated stakeholder describes longer delivery times in Abha and temporary perfume stock-outs. Those observations justify investigation, not a conclusion that one issue caused another.

Next, I would examine promotion profitability and customer-level retention before changing discounts or channel spending.

## 13. Final Summary

### Analyst - English

Based on the information provided, summarize the key findings and give two practical recommendations.

### Business Stakeholder

### Key findings

- Sales grew from 420,000 to 505,000 SAR; orders rose from 1,240 to 1,430.
- Average order value increased from 339 to 353 SAR.
- Riyadh had the largest **absolute city revenue increase** (40,000 SAR), while Abha had the highest **percentage city growth** (34.88%).
- The website remained the largest channel by revenue; this does not establish the best conversion or profitability.
- Personalized gifts had the largest absolute product revenue increase (26,000 SAR), while flowers remained the top product by revenue.
- New customers increased from 780 to 910, while repeat customers declined from 430 to 410.
- Late delivery was the most common complaint, representing 33% of complaints.
- The fictional scenario mentions discounts, stock constraints, and delivery delays. The available aggregates cannot show their causal effect on sales, profit, or repeat purchasing.

### Two recommendations

1. Investigate fulfillment: measure delivery performance by city and courier, review stock availability for perfumes and gift materials, and monitor personalization quality.
2. Evaluate profitable retention before changing promotions: track margin, discount costs, repeat-purchase cohorts, and customer acquisition cost by channel.
