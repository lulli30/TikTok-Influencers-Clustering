# TikTok Influencer Clustering (2025)

This project applies **DBSCAN clustering** to identify patterns among the **Top 100 TikTok influencers in 2025**, based on their **Followers, Likes, and Uploads**. The dataset is processed, clustered, and visualized to provide insights into different influencer categories.

## Features
- **DBSCAN Clustering**: Automatic grouping of influencers without predefined categories.
- **Silhouette Score Optimization**: Grid search to find the best `eps` and `min_samples` values.
- **Data Normalization**: StandardScaler ensures features have equal weight.
- **Cluster Labeling**: Meaningful names replace numeric cluster IDs.
- **Visualization**: Log-scale scatter plot for better cluster representation.

## Installation
Clone the repository and install the required libraries:
```bash
git clone https://github.com/yourusername/tiktok-influencer-clustering.git
cd tiktok-influencer-clustering
pip install -r requirements.txt
```

## Usage
1. **Prepare the dataset**: Place `Top_100_tiktokers_in_2025.csv` in the project folder.
2. **Run the script**:
    ```bash
    python clustering.py
    ```
3. **View results**: The updated dataset `Updated_Top_100_TikTok_Influencers_2025.csv` will be generated.

## Sample Data (First 5 Rows)

| Rank | Username        | Followers  | Following | Uploads | Likes       | Cluster | Cluster_Label              |
|------|---------------|------------|-----------|---------|------------|---------|----------------------------|
| 1    | Khabane lame  | 162400000  | 78        | 1251    | 2500000000  | -1      | Outliers (High Followers)  |
| 2    | charli d'amelio | 155700000  | 1304      | 2812    | 11800000000 | -1      | Outliers (High Followers)  |
| 3    | MrBeast       | 107500000  | 362       | 394     | 1100000000  | -1      | Outliers (High Followers)  |
| 4    | Bella Poarch  | 94300000   | 649       | 771     | 2400000000  | -1      | Outliers (High Followers)  |

## Output
- Clustered dataset with meaningful labels.
- Identified **outliers** (influencers with extreme popularity).
- Visualized influencer clusters.

## Contributing
Feel free to submit pull requests or raise issues for improvements.

## License
MIT License

