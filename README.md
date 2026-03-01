# Lab Assignment 01: Data Preprocessing
## Data Mining and Its Applications

### Group Information
- **Group ID:** 05
- **Members:**
  - Bùi Minh Duy - 23127040
  - Phi Anh Khôi - 23127073
  - Lê Minh Đức - 23127351

### Assignment Overview
This project focuses on data preprocessing techniques for different types of data:
- **Part 1 (Required):** Image Data Preprocessing
- **Part 2 (Required):** Tabular Data Preprocessing
- **Part 3/4 (Bonus - Choose One):** Text or Temporal Data Preprocessing

### Datasets Used

#### Part 1: Image Data
- **Dataset:** Chest X-Ray Pneumonia
- **Source:** https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia
- **Description:** 5,863 chest X-ray images (JPEG) in 2 categories: Pneumonia and Normal, organized into train/test/val splits

#### Part 2: Tabular Data
- **Dataset:** Car Resale Data - 2023
- **Source:** https://www.kaggle.com/datasets/rahulmenon1758/car-resale-prices
- **Description:** 17,446 records with 15 attributes about used car listings in India (price, engine, mileage, fuel type, etc.); target variable is resale_price

#### Part 3: Text Data (Bonus)
- **Dataset:** IMDB Dataset of 50K Movie Reviews
- **Source:** https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews
- **Description:** 50,000 IMDB movie reviews labeled as positive or negative for sentiment analysis

#### Part 4: Temporal Data (Bonus)
- **Dataset:** NASDAQ Stock Market Data (AAPL)
- **Source:** https://www.kaggle.com/datasets/jacksonce/stock-market-dataset
- **Description:** Daily AAPL stock prices from 1980 to 2022 (40+ years) including Open, High, Low, Close, Adjusted Close, and Volume

### Project Structure
```
Lab01/
├── README.md                          # This file
├── requirements.txt                   # Python dependencies
├── data/                             # Data directory
│   ├── images/                       # Image datasets
│   ├── tabular/                      # Tabular datasets
│   ├── text/                         # Text datasets (if applicable)
│   └── temporal/                     # Time-series datasets (if applicable)
├── notebooks/                        # Jupyter notebooks
│   ├── 01_image_preprocessing.ipynb         # Part 1 (Required)
│   ├── 02_tabular_preprocessing.ipynb       # Part 2 (Required)
│   ├── 03_text_preprocessing.ipynb          # Part 3 (Bonus)
│   └── 04_temporal_preprocessing.ipynb      # Part 4 (Bonus)
└── docs/                             # Documentation
    └── Report.pdf                     # Final report
```

### Installation & Setup

#### 1. Create Python Virtual Environment (Recommended)

A virtual environment keeps your project dependencies isolated and prevents conflicts with other projects.

```bash
# Navigate to project directory
python -m venv .venv

# Activate virtual environment
# On Windows:
.venv\Scripts\activate

# On macOS/Linux:
source .venv/bin/activate
```

#### 2. Install Python Dependencies

With the virtual environment activated:

```bash
# Upgrade pip first (recommended)
python -m pip install --upgrade pip

# Install all required packages
pip install -r requirements.txt
```

#### 3. Download Datasets

- Download all datasets from the Google Drive link below:
  - **Google Drive:** https://drive.google.com/drive/folders/1ktw0bJKU2pjxvoPSB1UC9_NDBxa3u5qO
- Place datasets in the appropriate `data/` subdirectories:
  - `data/images/` - for image datasets
  - `data/tabular/` - for tabular datasets
  - `data/text/` - for text datasets
  - `data/temporal/` - for temporal datasets

### Running the Notebooks

1. Navigate to the project directory
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open notebooks in the `notebooks/` directory:
   - `01_image_preprocessing.ipynb` (Required - Part 1)
   - `02_tabular_preprocessing.ipynb` (Required - Part 2)
   - `03_text_preprocessing.ipynb` (Bonus - Part 3)
   - `04_temporal_preprocessing.ipynb` (Bonus - Part 4)
   
   **Note:** Choose either Part 3 or Part 4 for bonus (not both)

### External Resources
- **Google Drive (if datasets > 25MB):** https://drive.google.com/drive/folders/1ktw0bJKU2pjxvoPSB1UC9_NDBxa3u5qO

### Assignment Details
- **Instructor:** MSc. Lê Nhựt Nam
- **Email:** lnnam@fit.hcmus.edu.vn

### License
This project is for educational purposes only as part of CSC14004 - Data Mining course at University of Science, VNU-HCMC.
