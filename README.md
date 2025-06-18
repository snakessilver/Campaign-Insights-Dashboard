# 📊 Campaign Insights Dashboard (Power BI + Python)

This project showcases a data-driven marketing dashboard built with **Power BI**, enhanced with **Python visuals** to analyze and optimize campaign performance across platforms.

> 💡 Ideal for roles involving **data analysis, marketing insights, or full-stack data reporting**.

---

## 🚀 Features

- 📈 **CTR (%) Comparison by Platform** — Python bar chart with custom styling.
- 💰 **Campaign Cost vs. Conversions** — Scatter plot to analyze performance efficiency.
- 🎯 **Top-Performing Platforms & Campaigns** — Identified via clean Power BI visuals.
- 🧠 **Embedded Python Visuals** — Used for customization, styling, and added analytical power.
- 🌙 **Dark Theme Dashboard** — Professional UI with bold fonts and color contrast.

---

## 🐍 Embedded Python Code Sample

```python
import matplotlib.pyplot as plt
import seaborn as sns

fig, ax = plt.subplots(figsize=(10,6))
fig.patch.set_facecolor('black')
ax.set_facecolor('black')

sns.barplot(x=dataset['Platform'], y=dataset['CTR (%)'], palette='coolwarm', ax=ax)

plt.title('CTR (%) by Platform', fontsize=16, fontweight='bold', color='white')
plt.xlabel('Platform', fontsize=14, color='white')
plt.ylabel('CTR (%)', fontsize=14, color='white')

ax.tick_params(axis='x', labelsize=11, colors='white')
ax.tick_params(axis='y', labelsize=11, colors='white')

plt.xticks(rotation=45)
plt.tight_layout()
plt.show()

