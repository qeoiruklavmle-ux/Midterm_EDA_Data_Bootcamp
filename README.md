# Bootcamp Midterm EDA Case Study: 
# Labor Productivity Slowdown in the United States 
## Capital Investment vs Technological Progress

**Author:** Helen Jeon

---

## Repository Structure

| File | Description |
| :--- | :--- |
| Jeon_Helen_Productivity_Growth.ipynb | Project Notebook: The consolidated version used to generate visualizations and statistical insights for the case. |
| Productivity Growth USA All Measures.csv | Dataset: OECD productivity dataset containing U.S. growth measures. Serves as the primary data source for all exploratory analysis and growth accounting in this project. |
| README.md | Documentation: The main landing page explaining project scope and findings. |

---

## Definitions

* Labor Productivity: Efficiency of labor inputs in conjunction with other factors of production (capital and multifactor productivity).  
* Capital Deepening: Refers to an increase in the proportion of the capital stock to the number of labor hours worked.
* Multifactor Productivity: Reflects the overall efficiency of combining labor and capital inputs (interchangeable with technological progress in this case).
* ICT Capital: Acquisition of equipment and computer software (technology) that is used in production for more than one year.

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

### 2. Productivity is strongly linked to MFP
- Strong correlation between productivity and MFP (~0.88)  
- Slightly weaker but still strong correlation with capital (~0.80)
- Productivity closely follows MFP patterns  

**This suggests MFP plays a stronger role in productivity changes.**

### 3. Pre vs Post 2000 comparison
- Capital contribution is relatively stable
- MFP remains large but inconsistent  

**The slowdown is driven by instability, not disappearance of capital inputs.**

---

## Introduction

### Labor Productivity Growth Over Time
Productivity growth is a key driver of long-term economic performance, influencing wages, living standards, and overall economic prosperity. In recent decades, however, the United States has experienced a noticeable slowdown in productivity growth, raising questions about its underlying causes.

Understanding the slowdown in U.S. productivity growth begins with examining how productivity has evolved over time.  Identifying long-term trends in productivity growth is therefore a critical first step in determining whether a structural slowdown has occurred.

Figure 1: U.S. Productivity Growth Rates Over Time

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/4f7e4c1c-9b5d-451e-a328-669a8abb3984" />

*	Productivity is cyclical and volatile
    *	There are frequent spikes and drops, meaning productivity growth is not stable and varies year to year
*	Strong growth in the late 1990s / early 2000s
    *	This aligns with the tech/IT boom, when computers and the internet boosted efficiency.
*	Noticeable slowdown after the early 2000s
    *	Growth mostly stays around ~1% or lower

### Distribution of Labor Productivity Growth Rates Pre and Post 2000
To further understand the nature of the slowdown, it is important to examine how the distribution of  growth rates has changed over time. Figure 2 quantifies this change through percentile analysis. Comparing key points in the distribution, such as the 25th, 50th (median), and 75th percentiles, determines whether the slowdown is concentrated in certain segments or reflects a broader structural shift.

Figure 2: Shift in U.S. Productivity Growth Across Percentiles (Pre- vs Post-2000)

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/6d813c72-b37d-4e1f-b98b-1b411189c483" />

Table 1: Comparison of U.S. Productivity Growth Percentiles (Pre- vs Post-2000)

| Percentile | Pre-2000 (%) | Post-2000 (%) | Difference |
| :--- | :--- | :--- | :--- |
| 25th |	0.963	| 0.915	| 🔻 -0.049 |
| 50th (Median) |	1.639	| 1.191	| 🔻 -0.449 |
| 75th	| 2.314 |	1.778	| 🔻 -0.537 |

The comparison of percentiles shows a clear downward shift in the distribution of productivity growth. The median growth rate declined significantly from 1.64% to 1.19%, while the 75th percentile also fell by more than 0.5 percentage points (Table 1). This indicates that not only has typical productivity growth weakened, but even the strongest growth periods are less robust than before. Therefore, the slowdown reflects a broad structural decline.

## Analysis

### Factors of Labor Productivity Growth

To understand the underlying drivers of the broad structural slowdown, the project investigates  the relationships between productivity and its key inputs. In particular, capital deepening and technological progress represent the primary channels through which productivity evolves over time. The following correlation matrix in Figure 3 highlights how closely productivity growth is associated with these factors, providing insight into whether changes in capital investment or technological progress play a more significant role in shaping productivity outcomes.

Figure 3: Correlation Between Productivity Growth, Capital Deepening, and MFP

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/ae59120e-ab1f-4eeb-9874-c206c97238ea" />

While the correlation matrix highlights a strong positive relationship between productivity growth, capital deepening, and multifactor productivity (MFP), the scatter plot in Figure 4 provides a more detailed view of how these variables interact. The positive relationship between productivity growth and capital deepening is evident, as higher levels of capital are generally associated with higher productivity. However, the inclusion of MFP as a third dimension reveals that observations with higher MFP consistently correspond to higher productivity outcomes, even at similar levels of capital. This suggests that while capital supports productivity, technological progress plays a critical role in amplifying its effects, reinforcing the idea that MFP is a key driver of productivity growth.

Figure 4: Relationship Between Productivity Growth and Capital Deepening with MFP

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/c1e412b1-1a5e-42bd-b9e1-ae84b55ab756" /> 

The comparison of growth rates over time in Figure 5 provides important insight into the drivers of productivity dynamics. While capital deepening exhibits higher overall growth rates, it is also significantly more volatile and does not closely track changes in productivity. In contrast, productivity growth aligns more closely with trends in multifactor productivity (MFP), particularly during periods of both expansion and slowdown. Notably, the decline in productivity (2005 - 2008) coincides with weaker and more inconsistent MFP growth, despite continued contributions from capital. This suggests that fluctuations in technological progress play a more critical role in driving changes in productivity growth over time.

Figure 5: Growth Rates of Productivity, Capital Deepening, and MFP Over Time

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d8478b4f-75ca-41c7-9fda-0c16b1b0ee6b" />

### Growth Accounting Decomposition

To quantify how much each factor contributes to overall productivity growth and isolate these effects, a growth accounting framework can be used to decompose productivity into contributions from capital and technological progress. 

The Solow model suggests that labor productivity growth rate (Y/L) is broken down into two components: 
* Contribution from capital deepening (K/L) (weighted by α)
* Technological progress growth (A)

<img width="476" height="122" alt="Screenshot 2026-03-26 at 17-12-55 solow labor productivity growth equation - Google Search" src="https://github.com/user-attachments/assets/91c67709-c88b-435a-b0c1-012cbf167a8b" />

Figure 6 presents an OECD-based growth accounting decomposition of productivity. While capital provides a relatively stable foundation, fluctuations in productivity closely mirror changes in MFP, particularly during periods of slowdown and recovery. This suggests that variations in technological progress, rather than capital investment, play a more significant role in driving changes in productivity growth over time.

Figure 6: Growth Accounting Decomposition of Productivity Growth

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/35d8e3a8-09fa-4e28-85ef-92bc549780bd" />

### Additional Insight into Capital Contribution

Further decomposition of capital reveals that not all forms of investment contribute equally to productivity growth. Figure 7 shows that ICT-related capital provides a more stable and consistently positive contribution, while non-ICT capital is more volatile and less reliable over time. This suggests that technology-oriented investment plays a more important role in supporting sustained productivity growth than traditional forms of capital.

Figure 7: ICT and Non-ICT Capital Contributions to Productivity Growth Over Time

<img width="500" height="500" alt="Untitled" src="https://github.com/user-attachments/assets/af4a2e9d-8efb-4460-abd8-a08ef8d01d24"/>

---

## Conclusion

The slowdown in U.S. productivity growth is not primarily driven by weaker capital investment. Capital deepening remains relatively stable and continues to contribute to productivity.

Instead, the slowdown is more closely linked to changes in multifactor productivity (MFP). MFP is volatile and plays a dominant role in driving productivity fluctuations. When productivity weakens, it is largely due to weaker or inconsistent MFP contributions rather than reduced capital.

Additionally, ICT capital contributes more consistently than non-ICT capital, highlighting the importance of technology-related investment.

Overall, the slowdown reflects a decline in the efficiency and consistency of technological progress rather than a lack of capital.

---

## Final Insight

The key challenge for the U.S. economy is not generating more capital, but ensuring that technological progress and innovation are effectively translated into sustained productivity growth.
