
# ⭕️ VennLit

VennLit allows generation of Venn diagram for comparison of 2 or 3 sets of data for similarities and differences.

## Demo App

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://vennlit.streamlit.app/)

## GitHub Codespaces

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/dataprofessor/vennlit?quickstart=1)
---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Data Format](#data-format)
- [Sample Data](#sample-data)
- [Quick Start](#quick-start)
- [Technologies](#technologies)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

VennLit is a simple yet powerful tool built with Streamlit that helps you create professional Venn diagrams for data comparison. Whether you're analyzing gene sets, comparing text documents, or finding common elements between datasets, VennLit provides an intuitive interface to visualize relationships between multiple sets.

---

## ✨ Features

- **2-Set Venn Diagrams**: Compare two datasets to identify unique and common elements
- **3-Set Venn Diagrams**: Analyze three datasets simultaneously with detailed intersection counts
- **Multiple Input Methods**:
  - Manual text input
  - Load sample data
  - Space or line-separated values
- **Data Cleaning**: Automatic removal of quotes and extra whitespace
- **Interactive UI**: User-friendly Streamlit interface
- **Customizable Visualization**: Clear, easy-to-read diagrams
- **Count Display**: Automatic calculation of intersection sizes

---

## 📦 Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/dataprofessor/vennlit.git
   cd vennlit
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   
   - **Windows:**
     ```bash
     venv\Scripts\activate
     ```
   
   - **macOS/Linux:**
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 Usage

### Running the Application

```bash
streamlit run streamlit_app.py
```

The app will open in your default browser at `http://localhost:8501`

### How to Use

1. **Select the number of sets**: Choose between comparing 2 or 3 datasets
2. **Input your data**: 
   - Paste data directly into the text areas
   - Use the sample data button to load example datasets
3. **View the diagram**: The Venn diagram updates automatically as you input data
4. **Analyze results**: View the intersection counts and relationships

---

## 📝 Data Format

### Supported Formats

- **Space-separated**: `apple banana orange grape`
- **Newline-separated**: 
  ```
  apple
  banana
  orange
  ```
- **Comma-separated**: `apple, banana, orange`
- **With quotes**: `"apple" "banana" "orange"` or `'apple' 'banana' 'orange'`

### Data Processing

- Text is automatically trimmed of extra whitespace
- Quotes are removed for clean processing
- Empty items are filtered out
- Case-sensitive comparison

---

## 📚 Sample Data

Sample data files are included in the `data/` directory:

- `list_a.txt`: First set of sample items
- `list_b.txt`: Second set of sample items
- `list_c.txt`: Third set of sample items

### Loading Sample Data

Click the **"Load Sample Data"** button in the app to populate the text areas with example datasets.

---

## ⚡ Quick Start

### 1. Simple 2-Set Comparison

```
Set A: apple banana orange grape
Set B: banana orange lemon
Result: Venn diagram showing 2 common items (banana, orange)
```

### 2. Three-Set Analysis

```
Set A: python java javascript
Set B: java javascript ruby
Set C: javascript ruby golang
Result: Venn diagram showing programming language overlaps
```

---

## 🛠️ Technologies

| Technology | Purpose |
|-----------|---------|
| **Streamlit** | Web application framework |
| **Matplotlib** | Data visualization |
| **matplotlib-venn** | Venn diagram generation |
| **Pandas** | Data manipulation (optional) |
| **Python 3.8+** | Programming language |

---

## 📋 Requirements

See [requirements.txt](requirements.txt) for full dependency list: install in computer system python 3.12 or above version must be needed for run this and ide vscode , pycharm etc ... any of them you can use .

```
streamlit
matplotlib
matplotlib_venn
pandas
```

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Areas for Improvement

- Add support for more than 3 sets
- Export diagrams as images
- Add statistics and analysis features
- Support for different data formats (JSON, CSV)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🔗 Additional Resources

- [Streamlit Documentation](https://docs.streamlit.io/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Venn Diagrams on Wikipedia](https://en.wikipedia.org/wiki/Venn_diagram)

---

## 💡 Tips & Tricks

- **Preprocessing**: Clean your data before pasting to ensure accurate results
- **Large Datasets**: Works best with 100-1000 items per set
- **Performance**: For very large datasets (10,000+ items), results may be slow
- **Copy/Paste**: Easily copy results for documentation or reporting

---

## 🐛 Troubleshooting

### App won't start
```bash
# Ensure all dependencies are installed
pip install -r requirements.txt

# Try clearing Streamlit cache
streamlit cache clear
```

### Data not loading
- Check file paths are correct
- Ensure data files are in UTF-8 encoding
- Verify no special characters are causing issues

### Diagram not displaying
- Ensure at least 1 item in each set
- Check for empty or whitespace-only entries

---

## 📞 Support

For issues, questions, or suggestions:
- Open an issue on [GitHub Issues](https://github.com/dataprofessor/vennlit/issues)
- Check existing documentation and FAQs

---

**Happy comparing! 🎉**

