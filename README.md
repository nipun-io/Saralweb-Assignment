# SaralWeb SDE Assignment - Nov 2025

## 🧩 Problem Statement
You are given an array of time ranges `[start, end)` representing when a system was active.  
Each range includes `start` but excludes `end`.  
Ranges may overlap or be separated by small gaps.  
If a gap is smaller than a given `threshold` (in milliseconds), it should be treated as continuous and merged.

Implement a function:

```js
mergeTimeRanges(ranges, threshold)
```

that merges such ranges into non-overlapping, sorted intervals.

---

## 🧠 Implementation Logic
1. Sort the ranges by their start time.  
2. Initialize the first range as the current active range.  
3. Iterate through each range:
   - If the next range overlaps or the gap ≤ threshold → merge them.  
   - Otherwise, push the current range to the result and move on.  
4. Push the final active range.  
5. Return the merged array.

---

## 📁 Project Structure
```
├── my-module.js      # Node.js module containing mergeTimeRanges implementation
├── test.js           # Example test script
└── package.json      # Node.js module configuration
```
