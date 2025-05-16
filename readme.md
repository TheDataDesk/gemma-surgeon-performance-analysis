# Surgeon Performance Analysis  

*Gemma Analytics – Analytics Engineer Task*

This project analyzes EQ-5D-5L patient surveys to identify the most and least skilful surgeons for hip replacement operations, based on how much their patients improved after surgery.

---

## Objective

Measure patient improvement and rank surgeons by performance using a metric that combines:
- Average improvement
- Number of patients treated
- Consistency (via standard deviation)

---

## Approach

- Filtered for **hip surgeries**
- Mapped answers to numeric scores
- Calculated patient improvement (post - pre)
- Aggregated by surgeon
- Ranked using a **weighted score**:
      > avg_improvement × log(1 + num_patients)

---

## Highlights

**Top Surgeons**: Obi-Wan Kenobi, Luke Skywalker, Mon Mothma  
**Lowest Ranked**: Padme Amidala, Princess Leia, Darth Maul

---

## Visuals

- Bar chart: Top 10 surgeons vs average improvements
![Barchart-surgeon_by avgimprovement](https://github.com/user-attachments/assets/0cf7d783-f8c8-400a-a53b-b30a0a1fa6ff)

- Bubble chart: Volume vs. improvement
![Bubbleplot-patientvol_avgimprovement](https://github.com/user-attachments/assets/d174ad54-7680-4329-95d2-9a5a951fccdb)

- Box plot: Outcome consistency ( surgeon vs improvement score) 

![Boxplot-improvementdistribution_bysurgeon](https://github.com/user-attachments/assets/260703fb-0b26-43f0-8804-6dbe3fc06036)

- Heatmap: Surgeon performance metric correlations 

![Heatmap-surgeonperformancemetrics](https://github.com/user-attachments/assets/fa612ef5-31e1-496e-9218-8b68c93a4865)

- BarChart: Patient Volume Vs Surgeons

![Barchart-patientvol_bysurgeon](https://github.com/user-attachments/assets/5bcd01d7-28ad-4683-8d7c-27596cef722c)

- BarChart: Surgeon Ranking based on weighted score
![BarChart-finalranking](https://github.com/user-attachments/assets/1baf1fc8-5a08-4621-980f-d19cd3bfdcdd)


**Note:** GitHub does not render interactive Plotly charts in Jupyter notebooks.  
> To view all visualizations, please refer to the static images in the `plots/` folder. 
---

## Tools

- Python, Pandas, NumPy  
- pandasql (SQL in Python)  
- Plotly (interactive charts)

---

##  How to Run

This project was built using **Python 3.9+**.

Make sure you're using Python 3.9 or higher. Then install the required packages and launch the notebook:

 ```bash
pip install -r requirements.txt
jupyter notebook
 ```
---

##  Final Note

Thank you for the opportunity to work on this challenge. I really enjoyed combining SQL, Python, and clear storytelling, especially knowing that Gemma values turning data into meaningful, actionable insights. I admire Gemma Analytics's mission to make analytics accessible and would be excited to contribute to that kind of work


