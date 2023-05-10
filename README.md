# Reeva-R
## Poster presentation exploring reasons behind weak service provision in the world. 
Welcome to this poster that explores the effects of economic inequality, security apparatus, and demographic pressures on service provision.
The poster introduces you to some skills to complete a poster on R-mardown `poster html`.
This project was intended for class. I asked and answered an empirical question using data from `The Fund for Peace's Fragile States Index (FSI)`. The challenge was to present the work in one poster to shed light on the impacts of weak security and economic inequality in addition to demographic pressures on service delivery in the world. 

## Data

The data presented in this report was collected from **The Fund for Peace's Fragile States Index `(FSI)`** which is an important instrument for identifying weaknesses that raise the possibility of state fragility. The information is based on twelve CAST framework indicators that are further divided into sub-indicators. Along with cross-cutting indicators of:
- **Social indicators:** The Demographic Pressures Indicator. 

Our data builds on three major indicators: 

- **Cohesion:** The Security Apparatus. 

- **Economic:** In general, Economic indicator takes into account aspects of a nation's economic deterioration. 

- **Political indicators:**  The Public Services Indicator describes the existence of fundamental government operations that benefit the populace. 

Before using any data, extensive efforts were made to ensure its quality and reliability. Data was carefully curated, cleaned, and processed to ensure consistency and accuracy.

Overall, this report provides a comprehensive analysis of the data collected and offers valuable insights into the research topic.

`Poster` includes the following elements: 

- Title.
- Author name.
- Introduction with main question, expectations, and importance.
- Data: source and brief description (graph and summary of key vars).
- Analysis: Pearson statistical test was used to evaluate hypotheses and correlation of our variables. The poster contains two tables and two visuals.
- Findings.

## Favourite Code Chunk

I write the following code to order to show the 2021 perceived shortage in Public Service delivery in 38 countries (from low to high on a scale of 10). 
Please make sure to follow all the steps on the `https://github.com/Selmamallem/Reeva-R/blob/main/poster.Rmd` **Poster.Rmd file** to be able to make the ggplot.  
```python
limit <- max(abs(my_data_desc$P2)) * c(-1, 1)

ggplot(my_data_desc, aes(reorder(Country, P2), P2)) + 
  geom_col(aes(fill = P2)) +
  theme_minimal() +
    labs( x = "Country",  
          y = "Public Services shortage (P2)") +
    scale_fill_scico(palette = "cork", limit = limit,
                    midpoint = median(my_data_desc$P2)) + 
  coord_flip() + 
  labs(x = "Country") 
  ```
  ![myprettycode-1](https://github.com/Selmamallem/Reeva-R/assets/123516651/53cb4759-2495-4612-b031-9f3f6fac82ec)
  
 *Thank you for taking the time to explore this poster, and I hope it inspires further discussion to improve it.*





