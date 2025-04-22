

# 🍽️ Zomato Restaurant Data Analysis

This project involves the exploration and visualization of Zomato restaurant data to derive key insights about restaurant ratings, costs, and customer preferences.

## 📁 Dataset

The dataset (`Zomato-data-.csv`) contains information about 148 restaurants, including:

- **Name** of the restaurant  
- Whether they accept **online orders** and **table bookings**  
- **Rating** and number of **votes**  
- **Approximate cost** for two people  
- Type of listing (e.g., **Buffet**, **Dining**, **Cafes**, etc.)

## 🧰 Libraries Used

- `pandas` for data manipulation
- `numpy` and `statistics` for calculations
- `matplotlib` and `seaborn` for data visualization

## 🔍 Key Analyses

### 📊 General Data Info & Cleaning
- Removed `/5` from the rating column and converted it to `float`.
- Handled formatting issues in the "approx_cost(for two people)" column.
- Converted cost to numeric for accurate analysis.

### 📈 Visual Insights

1. **Distribution by Type**  
   - Most restaurants are listed as **Dining** type.

2. **Average Cost per Restaurant Type**  
   - **Buffet** restaurants are the most expensive.
   - **Dining** is the most affordable.

   ![Average Cost Plot](#) <!-- You can embed screenshots here if uploading to GitHub -->

3. **Online Order Preferences**  
   - A majority of restaurants do **not** offer online ordering.

4. **Restaurant with Highest Votes**  
   - 🏆 *Empire Restaurant* has the highest number of votes (4,884).

5. **Rating vs Cost Relationship**  
   - Best-rated restaurants fall in the ₹700–800 range.

6. **Ratings Based on Online Ordering**  
   - Restaurants that accept **online orders** tend to have **higher ratings**.

7. **Top 5 Restaurants by Rating**
   - Includes restaurants like *Onesta*, *Empire Restaurant*, *Meghana Foods*, etc.

   ![Top Restaurants Bar Chart](#)

## 📌 Notable Observations

- Online-friendly restaurants are perceived better.
- Higher cost does not always guarantee higher ratings.
- Buffet types are pricier, but Dining options offer better affordability.

## ⚠️ Known Warnings

- Seaborn color palette usage may cause a `FutureWarning` due to deprecation of `palette` without `hue`.
- Adjusting the number of colors in custom palettes is recommended to avoid `UserWarning`.

## 🧠 Future Work

- Expand dataset to include more restaurants or different cities.
- Use NLP on reviews (if available) to enhance sentiment-based rating predictions.
- Implement machine learning models to predict ratings or preferred restaurant types.

## 🖥️ How to Run

1. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

2. Replace the file path with your local CSV file path:
   ```python
   df = pd.read_csv(r"path_to_your_file.csv")
   ```

3. Run the Jupyter notebook or Python script.

