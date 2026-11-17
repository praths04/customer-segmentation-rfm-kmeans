# Customer Segmentation for an Online Handloom Marketplace: RFM and K-Means

A customer segmentation project on about 35,000 e-commerce orders from an Indian handloom and handicraft marketplace. We cleaned and engineered the order data, clustered customers with k-means on RFM-style features, and visualised the segments with PCA to decide which customer groups to target.

**Tools:** Python (pandas, scikit-learn, Matplotlib, seaborn), Jupyter
**Type:** Team project, Johns Hopkins Carey Business School

---

## Question

Which groups of customers behave alike, and which of them should the business prioritise for marketing?

## Method

1. **Data cleaning:** removed duplicates (35,593 orders remained), checked for nulls, and dropped redundant columns (Total Sales, Gross Sales, Product Name).
2. **Feature engineering:** built customer-level features: Recency, Frequency, Monetary Value and Number of Discounts.
3. **Transformation:** encoded categorical fields and scaled the features to a common range before clustering.
4. **Choosing k:** used the elbow method and silhouette analysis across several values of k, and proceeded with four clusters.
5. **Clustering and PCA:** ran k-means, reduced the features with PCA (two components capture almost all the variance) and plotted the segments in 2D and 3D. Component 1 mainly reflects Recency and Frequency, and Component 2 reflects Monetary Value and Number of Discounts.

## Files

| File | What it is |
|---|---|
| `gocoop_customer_segmentation.html` | Exported notebook with the code, outputs and visualisations. Download it and open it in a browser. |

## Data

The order data belongs to the business and is **not included**. Sample-row previews have been removed from the exported notebook, and the notebook shows only aggregate outputs and plots.

## Limitations

- The notebook is an HTML export, so the code can be read but not rerun directly.
- The elbow and silhouette plots point to a small number of clusters, and the choice of four involves judgement. A different k would give different segments.
- Segments describe past purchasing behaviour. They have not been tested on a later period.

## Authors

Prathiba Reddy, Haritha Kirana Kumar, Divyansh Mishra, Rudransh Naredi, Keshav Sarda, Kartik Bhargav
MS in Business Analytics & AI, Johns Hopkins Carey Business School
[LinkedIn](https://www.linkedin.com/in/prathiba-reddy-namireddy) | [Portfolio](https://6a38b7b1cee129ca7a613700--comforting-queijadas-d1f251.netlify.app)
