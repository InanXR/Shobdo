# ProjectShobdo

![Project Shobdo Banner](assets/banner.png)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

**ProjectShobdo** is an open-source initiative dedicated to preserving and modernizing the Bengali language for the digital era. We provide a structured, high-quality corpus of over **45,000 Bengali words**, meticulously organized with meanings, pronunciations, parts of speech, and etymological data.

Designed for developers, linguists, and researchers, this dataset serves as a foundational layer for NLP tools, dictionary apps, and linguistic analysis.

---

## 📦 Dataset Formats

We distribute the dictionary in multiple industry-standard formats to ensure compatibility with your specific tech stack.

![Data Formats](assets/formats.png)

| Format | File Path | Ideal Use Case |
| :--- | :--- | :--- |
| **JSON** | [`dist/json/dictionary.min.json`](dist/json/dictionary.min.json) | Web Applications, REST APIs, NoSQL Databases |
| **CSV** | [`dist/csv/dictionary.csv`](dist/csv/dictionary.csv) | Data Science (Pandas/R), Spreadsheet Analysis |
| **SQL** | [`dist/sql/dictionary.sql`](dist/sql/dictionary.sql) | Mobile Apps (Android/iOS), Offline Storage |
| **XML** | [`dist/xml/dictionary.xml`](dist/xml/dictionary.xml) | Linguistic Research, TEI-Lite Compliance |

---

## 🚀 Quick Start

### For Developers (Node.js/JavaScript)
Integrate the raw JSON data directly into your application.

```javascript
const dictionary = require('./dist/json/dictionary.min.json');

// Example: Find a specific word
const wordData = dictionary.find(entry => entry.word === 'অভিধান');
console.log(wordData);

```

### For Researchers (Python)

Load the CSV dataset using Pandas for data analysis or NLP training.

```python
import pandas as pd

# Load the dictionary
df = pd.read_csv('dist/csv/dictionary.csv')

# Display the first 5 entries
print(df.head())

```

---

## 🛠️ Build from Source

The `dictionary.json` file serves as the **Single Source of Truth**. If you wish to modify the data or regenerate the distribution files (CSV, SQL, XML), follow these steps:

1. **Install Dependencies**
```bash
npm install

```


2. **Run Build Script**
```bash
npm run build

```



This command processes the source JSON and updates all files within the `dist/` directory automatically.

---

## 🤝 Contributing

Contributions are the heart of this project! We welcome fixes for typos, new word additions, or improvements to etymology data.

1. **Fork** the repository.
2. Edit `dictionary.json` (Do not edit files in `dist/` directly).
3. Run `npm run build` to verify your changes locally.
4. Submit a **Pull Request**.

---

## 📄 License

Copyright © 2025 InanXR.

This project is licensed under the **Apache License, Version 2.0** (the "License").

You may not use this file except in compliance with the License. You may obtain a copy of the License at:

http://www.apache.org/licenses/LICENSE-2.0

**Summary of Permissions:**

* ✅ **Commercial Use**
* ✅ **Modification**
* ✅ **Distribution**
* ✅ **Private Use**

**Conditions:**

* You must preserve the copyright and license notices.
* State changes made to the code.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

```

```
