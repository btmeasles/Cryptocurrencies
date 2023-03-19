# Cryptocurrencies

## Summary

---

The purpose of this lab was to plot cryptocurrencies by using an Unsupervised Machine Learning algorithm (specifically, K-Means) and their viability as an investment opportunity.

---

### Methodology:

---

- A *.csv* file was loaded into a Pandas DataFrame to be preprocessed for use in a K-Means algorithm. Any cryptocurrencies that were not actively being traded, or had not yet been mined, were dropped, as well as any rows with *Null* values.  
- After the name of every coin was moved to a separate DataFrame for future reference, the remaining ```object``` columns were converted to numeric values.  
- All values were then reduced to their Principal Compenents using the **PCA** algorithm, which were then used to fit a range of K-Means algorithms to find the *Elbow Curve*. 
- With the *Elbow Curve* showing an ideal fit of 4 components, the data is scaled, transformed, and fit to the K-Means algorithm. 
- The *Classes* found by the K-Means are added to the original, cleaned DataFrame, and all data is visualized using a scatter plot.