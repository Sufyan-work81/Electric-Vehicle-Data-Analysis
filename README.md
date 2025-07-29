# Electric Vehicle Data Analysis

## Overview
This repository contains a comprehensive analysis of electric vehicle specifications for 2025 models. The project explores key performance metrics, battery characteristics, efficiency, range, and other vital features of modern electric vehicles. Using Python's powerful data science stack, I've performed data cleaning, exploratory analysis, and visualization to uncover insights about the evolving EV market.

![Electric Vehicles](https://images.unsplash.com/photo-1554744512-6e0cdb8caaab?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1800&q=80)

## Key Features
- **Data Cleaning**: Handled missing values and data inconsistencies
- **Exploratory Analysis**: Examined distributions and relationships between key EV metrics
- **Brand Comparison**: Analyzed performance differences between manufacturers
- **Visualization**: Created insightful charts showing range, efficiency, and performance trends
- **Feature Engineering**: Derived new insights from existing data

## Dataset
The analysis uses the `electric_vehicles_spec_2025.csv` dataset containing specifications for 478 electric vehicle models from various manufacturers. Key features include:

- **Performance Metrics**: Top speed, acceleration, torque
- **Battery Specifications**: Capacity, type, number of cells
- **Efficiency Data**: Wh/km consumption, range
- **Physical Dimensions**: Length, width, height
- **Category Information**: Segment, drivetrain, body type

## Analysis Highlights

### Battery Capacity vs Range
![Battery Range](https://via.placeholder.com/600x400?text=Battery+Capacity+vs+Range+Chart)

The analysis reveals a strong positive correlation between battery capacity and vehicle range, with some manufacturers achieving better efficiency than others.

### Acceleration Performance by Brand
```python
# Top performing brands by acceleration
top_acceleration = ev.groupby('brand')['acceleration_0_100_s'].min().sort_values()
print(top_acceleration.head(5))

# Output:
# Porsche     2.2
# Tesla       2.5
# Lucid       2.7
# BMW         3.2
# Mercedes    3.5
```

### Efficiency Distribution
![Efficiency Distribution](https://via.placeholder.com/600x400?text=Efficiency+Distribution+Chart)

Most vehicles fall in the 140-180 Wh/km efficiency range, with premium models typically showing higher efficiency.

## Technologies Used
- **Python 3.9**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical operations
- **Matplotlib/Seaborn**: Data visualization
- **Scikit-learn**: Machine learning and data preprocessing
- **Plotly**: Interactive visualizations

## Getting Started

### Prerequisites
- Python 3.6+
- Jupyter Notebook
- Python data science stack (pandas, numpy, matplotlib, seaborn)

### Installation
1. Clone the repository:
```bash
git clone https://github.com/Sufyan786786/electric-vehicles-analysis.git
cd electric-vehicles-analysis
```

2. Create and activate a virtual environment:
```bash
python -m venv ev-env
source ev-env/bin/activate  # Linux/Mac
ev-env\Scripts\activate    # Windows
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Launch Jupyter Notebook:
```bash
jupyter notebook
```

## Usage
Open and run the `Electric_vehicles_data_Analyze.ipynb` Jupyter Notebook to:
1. Import and clean the dataset
2. Perform exploratory data analysis
3. Generate visualizations
4. Explore brand comparisons
5. Discover relationships between vehicle specifications

## Future Enhancements
- Add predictive modeling for vehicle range
- Incorporate pricing data analysis
- Develop interactive dashboards
- Include charging infrastructure analysis
- Implement time-series analysis of EV evolution

## Connect with Me
- **GitHub**: [Sufyan786786](https://github.com/Sufyan786786)
- **LinkedIn**: [Sufyan Anayat Ali](https://www.linkedin.com/in/sufyan-anayat-ali-90488a292)
- **Email**: portfoliosufyan@gmail.com

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Explore the future of transportation through data!** 🔋🚗💨
