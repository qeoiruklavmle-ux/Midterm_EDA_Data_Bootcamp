# Bootcamp Midterm EDA Case Study: 
# Labor Productivity Slowdown in the United States
## Capital Investment vs Technological Progress

**Author:** Helen Jeon

---

## Repository Structure

| File | Description |
| :--- | :--- |
| EDA_Case_Study.ipynb | Project Notebook: The consolidated version used to generate visualizations and statistical insights for the case. |
| Productivity Growth USA All Measures.csv | Dataset: OECD productivity dataset containing U.S. growth measures. Serves as the primary data source for all exploratory analysis and growth accounting in this project. |
| README.md | Documentation: The main landing page explaining project scope and findings. |

---

## Definitions

* Labor Productivity: Efficiency of labor inputs in conjunction with other factors of production (capital and multifactor productivity).  
* Capital Deepening: Refers to an increase in the proportion of the capital stock to the number of labor hours worked.
* Multifactor Productivity: Reflects the overall efficiency of combining labor and capital inputs (interchangeable with technological progress in this case).
* ICT Capital: Acquisition of equipment and computer software that is used in production for more than one year.

Source: OECD

---

## Summary

This analysis examines the slowdown in U.S. productivity growth over time and investigates whether it is driven by changes in capital investment or technological progress. Using time series trends, distribution shifts, correlation analysis, scatter relationships, and growth accounting decomposition, the results show a clear decline in productivity growth—especially after the early 2000s.

While capital deepening remains relatively stable and continues to contribute to productivity, technological progress (MFP) appears to play a more important role in explaining fluctuations and the observed slowdown. Additionally, further decomposition of capital reveals that ICT-related capital contributes more consistently to productivity than non-ICT capital, which is more volatile.

---

## Research Question

**To what extent can the slowdown in U.S. productivity growth be explained by changes in capital investment and fluctuations in multifactor productivity?**

---

## Key Findings

### 1. Clear slowdown in productivity growth over time
- Productivity growth peaks in the late 1990s to early 2000s  
- Significant decline after 2000, especially post-2008  
- Partial but volatile recovery after 2020  

**This indicates a structural slowdown rather than a temporary fluctuation.**

---

### 2. Productivity is strongly linked to MFP
- Strong correlation between productivity and MFP (~0.88)  
- Slightly weaker but still strong correlation with capital (~0.80)
- Productivity closely follows MFP patterns  

**This suggests MFP plays a stronger role in productivity changes.**

---

### 3. Pre vs Post 2000 comparison
- Capital contribution is relatively stable
- MFP remains large but inconsistent  

**The slowdown is driven by instability, not disappearance of capital inputs.**

---

## Introduction

### Labor Productivity Growth Over Time
Productivity growth is a key driver of long-term economic performance, influencing wages, living standards, and overall economic prosperity. In recent decades, however, the United States has experienced a noticeable slowdown in productivity growth, raising questions about its underlying causes.

Understanding the slowdown in U.S. productivity growth begins with examining how productivity has evolved over time.  Identifying long-term trends in productivity growth is therefore a critical first step in determining whether a structural slowdown has occurred.

Figure 1: Productivity Growth Rate

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/4f7e4c1c-9b5d-451e-a328-669a8abb3984" />

*	Productivity is cyclical and volatile
    *	There are frequent spikes and drops, meaning productivity growth is not stable and varies year to year
*	Strong growth in the late 1990s / early 2000s
    *	This aligns with the tech/IT boom, when computers and the internet boosted efficiency.
*	Noticeable slowdown after the early 2000s
    *	Growth mostly stays around ~1% or lower

To further understand the nature of the slowdown, it is important to examine how the distribution of  growth rates has changed over time. Figure 2 shows the distribution of productivity growth rates throughout 1960 to 2024, where observations are more spread out and include a higher concentration of moderate-to-high growth outcomes. In contrast, Figure 3 shows the distribution in the later period (1996 - 2024), which appears more concentrated around lower growth rates and includes fewer high-growth observations. This visual comparison suggests a leftward shift in the distribution of productivity growth, indicating that the slowdown is not limited to a few periods but reflects a broader change across the entire distribution.

Figure 2: Distribution of Productivity Growth Rates (1960 - 2024)

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/69d95978-ceff-412a-a481-6ab43f1b3718" />

Figure 3: Distribution of Productivity Growth Rates (1996 - 2024)

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/2786e3c1-b635-41e2-baef-1718b4152e9a" />

A more precise way to quantify this change is through percentile analysis (Figure 4). By comparing key points in the distribution, such as the 25th, 50th (median), and 75th percentiles, we can determine whether the slowdown is concentrated in certain segments or reflects a broader structural shift.

Figure 4:

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/6d813c72-b37d-4e1f-b98b-1b411189c483" />

Table 1:

| Percentile | Pre-2000 (%) | Post-2000 (%) | Difference |
| :--- | :--- | :--- | :--- |
| 25th |	0.963	| 0.915	| 🔻 -0.049 |
| 50th (Median) |	1.639	| 1.191	| 🔻 -0.449 |
| 75th	| 2.314 |	1.778	| 🔻 -0.537 |

The comparison of percentiles shows a clear downward shift in the distribution of productivity growth. The median growth rate declined significantly from 1.64% to 1.19%, while the 75th percentile also fell by more than 0.5 percentage points (Table 1). This indicates that not only has typical productivity growth weakened, but even the strongest growth periods are less robust than before. Therefore, the slowdown reflects a broad structural decline.


---

## Conclusion

The slowdown in U.S. productivity growth is not primarily driven by weaker capital investment. Capital deepening remains relatively stable and continues to contribute to productivity.

Instead, the slowdown is more closely linked to changes in multifactor productivity (MFP). MFP is volatile and plays a dominant role in driving productivity fluctuations. When productivity weakens, it is largely due to weaker or inconsistent MFP contributions rather than reduced capital.

Additionally, ICT capital contributes more consistently than non-ICT capital, highlighting the importance of technology-related investment.

Overall, the slowdown reflects a decline in the efficiency and consistency of technological progress rather than a lack of capital.

---

## Final Insight

The key challenge for the U.S. economy is not generating more capital, but ensuring that technological progress and innovation are effectively translated into sustained productivity growth.
