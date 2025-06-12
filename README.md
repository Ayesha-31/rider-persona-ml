
# Rider Persona Classification using Trip Data

This project demonstrates how to classify ride-hailing users into simplified personas based on behavioral features extracted from trip data.

## 👥 Personas
- **Worker**: Rides mostly during commute hours
- **Leisure**: Active at night or weekends
- **LowUsage**: Infrequent users with few signals

## 🧪 Data Used
### ✅ Synthetic Data
- Generated riders with clean behavioral patterns
- Clustered using KMeans (5 groups → simplified to 3)
- Classifier achieved **100% accuracy** due to clean separation

### 🔁 Real-World (NYC FHV Data)
- Used NYC TLC High Volume For-Hire Vehicle trip records
- Assigned rider_ids randomly to simulate usage
- Clustering and classification accuracy was significantly lower (17–20%) due to noise and overlapping behaviors

## 🧠 Features Used
- % of rides during commute hours
- % of rides at night
- % of rides on weekends
- % of shared rides
- Average trip miles and duration

## 🚀 Results
| Dataset      | Accuracy | Notes                              |
|--------------|----------|-------------------------------------|
| Synthetic    | 100%     | Cleanly separated behaviors         |
| Real-World   | ~17%     | Noisy data, overlapping patterns    |

## 📦 Files
- `rider_persona_classified.csv`: Final data with simplified persona labels
- `notebook.ipynb`: Full clustering + classification pipeline
- `README.md`: Project overview

## 🔮 Future Work
- Improve cluster interpretability on real data
- Try DBSCAN or Gaussian Mixture Models
- Deploy prediction as a Streamlit app

---

**Author:** [Your Name]
