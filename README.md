# Lab Assignment 01: Data Preprocessing
## Data Mining and Its Applications

### Group Information
- **Group ID:** [To be filled]
- **Members:**
  - [Name 1] - [Student ID]
  - [Name 2] - [Student ID]
  - [Name 3] - [Student ID]

### Assignment Overview
This project focuses on data preprocessing techniques for different types of data:
- **Part 1 (Required):** Image Data Preprocessing
- **Part 2 (Required):** Tabular Data Preprocessing
- **Part 3/4 (Bonus - Choose One):** Text or Temporal Data Preprocessing

### Datasets Used

#### Part 1: Image Data
- **Dataset:** [Dataset name to be selected]
- **Source:** [Dataset source URL]
- **Description:** [Brief description]

#### Part 2: Tabular Data
- **Dataset:** [Dataset name to be selected]
- **Source:** [Dataset source URL]
- **Description:** [Brief description]

#### Part 3/4: Text/Temporal Data (Bonus)
- **Dataset:** [Dataset name to be selected]
- **Source:** [Dataset source URL]
- **Description:** [Brief description]

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

#### 3. Download NLTK Data (Required for Text Preprocessing)

If you're doing Part 3 (Text), download required NLTK data:

```python
# Run this in Python or in a Jupyter notebook cell
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('averaged_perceptron_tagger')
```

#### 4. Download Datasets

- Follow the links in the respective notebook sections
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
- **Google Drive (if datasets > 25MB):** [Link to be added]
- **Additional Resources:** [Links to be added]

### Assignment Details
- **Instructor:** MSc. Lê Nhựt Nam
- **Email:** lnnam@fit.hcmus.edu.vn
- **Deadline:** 23:55 13/02/2026
- **Duration:** ~3 weeks

### Notes
- All documentation must be in Vietnamese
- Code must be well-commented and explained
- AI assistance limited to 30%
- Late submissions not accepted

### License
This project is for educational purposes only as part of CSC14004 - Data Mining course at University of Science, VNU-HCMC.
