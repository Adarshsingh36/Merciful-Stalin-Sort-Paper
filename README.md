## Stalin Sort: A Comparative Study

## 📘 About the Project

This repository contains the implementation and performance analysis of **Stalin Sort**, a humorous yet unconventional sorting algorithm. Stalin Sort aggressively removes any element from a list that violates the non-decreasing order, rather than attempting to rearrange them.

This project also explores a variant, **Merciful Stalin Sort**, which tries to reinsert misplaced elements rather than discarding them permanently.

📄 The full research paper is included in the `Stalin Sort paper.docx` file.

## 📌 Key Concepts

- **Stalin Sort**: Retains only the increasing subsequence by removing unordered elements.
- **Merciful Stalin Sort**: A more tolerant variant that considers reinsertion.
- Performance benchmarks against traditional sorting algorithms.
- Visualization and comparative graphs using Python.

## 📊 Algorithmic Comparison

| Algorithm            | Best Case | Worst Case |
|----------------------|-----------|------------|
| Stalin Sort          | O(n)      | O(n²)      |
| Merciful Stalin Sort | O(n)      | O(n log n) |
| Insertion Sort       | O(n)      | O(n²)      |
| Selection Sort       | O(n²)     | O(n²)      |
| Merge Sort           | O(n log n)| O(n log n) |

## 🧠 Pseudocode - Stalin Sort

```python
def stalin_sort(arr):
    if not arr:
        return []
    result = [arr[0]]
    for i in range(1, len(arr)):
        if arr[i] >= result[-1]:
            result.append(arr[i])
    return result
```

## 💡 Use Cases

- **Data filtering**: Extract clean, increasing subsequences.
- **Ranking systems**: Automatically eliminate lower, unordered scores.
- **Data validation**: Identify and remove anomalies.

## 🧪 Experimental Setup

- Written in Python 3
- Graphs generated with Matplotlib and NumPy
- Test cases include:
  - Random arrays
  - Pre-sorted arrays
  - Reverse-sorted arrays

## 📂 Project Structure

```
📁 stalin-sort-research/
├── Stalin Sort paper.docx
├── DAA PAPER.pdf
├── stalin_sort.py
├── merciful_stalin_sort.py
├── graphs/
│   ├── complexity_plot.png
│   └── comparison_chart.png
└── README.md
```

## 🔧 Requirements

- Python 3.8+
- `matplotlib`, `numpy`

Install dependencies:
```bash
pip install matplotlib numpy
```

## 📃 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 📬 Contact

If you found this interesting or useful, feel free to reach out or collaborate!

---

*For educational purposes only. Not suitable for real-world production sorting tasks.*
```

---

Would you like me to tailor this more towards developers (with CLI usage and outputs), students (with learning outcomes), or meme/humor enthusiasts?# Merciful-Stalin-Sort-Paper
