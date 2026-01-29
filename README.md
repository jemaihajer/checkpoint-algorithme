# Sentence Analyzer Algorithm - Checkpoint

## 📋 Overview
This repository contains an algorithm that analyzes a sentence character by character and determines:
- The **length** of the sentence (total number of characters including the period)
- The **number of words** in the sentence (words separated by single spaces)
- The **number of vowels** in the sentence (a, e, i, o, u - both uppercase and lowercase)

## 🎯 Checkpoint Requirements
This algorithm was developed as part of the "Introduction to Algorithms" checkpoint with the following specifications:
- Read a sentence character by character
- The sentence must end with a period (`.`)
- Use **three variables as counters** to track:
  1. Sentence length
  2. Word count
  3. Vowel count
- Each character is treated separately

## 🔧 Algorithm Logic

### Variables Used
The algorithm uses three counter variables as required:
1. `length` - Counts every character in the sentence (including the period)
2. `word_count` - Counts the number of words (initialized to 1, increments on spaces)
3. `vowel_count` - Counts all vowels (both uppercase and lowercase)

### How It Works
1. **Input Phase**: The algorithm prompts the user to enter a sentence ending with a period
2. **Processing Phase**: 
   - Reads each character one by one using a REPEAT-UNTIL loop
   - For each character:
     - Increments the `length` counter
     - Checks if it's a space and increments `word_count` if true
     - Checks if it's a vowel (a, e, i, o, u, A, E, I, O, U) and increments `vowel_count` if true
   - Continues until a period (`.`) is encountered
3. **Output Phase**: Displays all three results to the user

## 📝 Example Execution

**Input:**
```
Hello world.
```

**Output:**
```
--- Sentence Analysis Results ---
Length of the sentence (including the period): 13
Number of words in the sentence: 2
Number of vowels in the sentence: 3
```

**Breakdown:**
- **Length**: H-e-l-l-o-[space]-w-o-r-l-d-. = 13 characters
- **Words**: "Hello" and "world" = 2 words
- **Vowels**: e, o, o = 3 vowels

## 🚀 How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/checkpoint-algorithms.git
   ```

2. Open the `checkpoint.algo` file in your algorithm editor/environment

3. Run the algorithm and enter a sentence when prompted (make sure to end with a period)

4. View the analysis results

## 📂 Repository Structure
```
checkpoint-algorithms/
├── checkpoint.algo    # Main algorithm file
└── README.md         # This documentation file
```

## 💡 Key Features
- ✅ **Character-by-character processing**: Each character is read and analyzed individually
- ✅ **Three counter variables**: Meets the requirement of using exactly three counters
- ✅ **Vowel detection**: Recognizes both uppercase and lowercase vowels
- ✅ **Space-based word counting**: Assumes words are separated by single spaces
- ✅ **Period termination**: Algorithm stops when it encounters the period
- ✅ **Clear documentation**: Well-commented code for easy understanding

## 📊 Algorithm Complexity
- **Time Complexity**: O(n) - where n is the number of characters in the sentence
- **Space Complexity**: O(1) - uses only three counter variables plus one character variable

## 🔍 Assumptions
- Words are separated by **single spaces** (no multiple consecutive spaces)
- The sentence **must end with a period** (`.`)
- Vowels include: a, e, i, o, u (both uppercase and lowercase)
- All characters count toward the length, including spaces and the period

## 📖 Learning Outcomes
This checkpoint demonstrates:
- Understanding of basic algorithm structure
- Character-by-character input processing
- Use of counters and control flow
- Conditional logic (IF statements)
- Loop control (REPEAT-UNTIL)
- Problem decomposition into smaller tasks

## 📅 Checkpoint Information
- **Deadline**: October 29, 2025
- **Course**: Introduction to Algorithms
- **Topic**: Algorithms and its elements

## 👨‍💻 Author
Created as part of the Software Development Bootcamp curriculum.

---

**Note**: This algorithm is designed for educational purposes to demonstrate fundamental algorithmic thinking and problem-solving skills.
