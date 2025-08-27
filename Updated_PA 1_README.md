# PA 1 – Python Practice Problems

Welcome! 👋  
This document will guide you through three beginner-friendly Python problems, showing you how the code works step-by-step. Feel free to run the code snippets and play with different inputs!

---

## 1. 🥣 Alphabet Soup

**Goal:**  
Rearrange the letters of a word in alphabetical order.

### How does it work?

1. **Define a function:**  
   Create a function named `alphabet_soup` that takes a word (string) as input.

2. **Sort the letters:**  
   Use Python’s built-in `sorted()` function to alphabetize the letters in the word.

3. **Join the letters back together:**  
   The `sorted()` function returns a list, so use `''.join()` to turn it back into a string.

4. **Print the result:**  
   Call the function with your word and print the result.

```python
def alphabet_soup(word):
    # Step 2 & 3: Sort and join the letters
    return "".join(sorted(word))

# Step 4: Try it out!
print(alphabet_soup("hello"))   # Output: 'ehllo'
print(alphabet_soup("hacker"))  # Output: 'acehkr'
```

**Try changing the input words to see what happens!**

---

## 2. 😊 Emoticon Replacer

**Goal:**  
Automatically replace emotion words in a sentence with their emoticons.

### How does it work?

1. **Define a function:**  
   Create a function named `emotify` that takes a sentence as input.

2. **Replace words with emoticons:**  
   Use `.replace()` to swap out emotion words for emoticons:
   - "smile" → `:)`
   - "grin"  → `:D`
   - "sad"   → `:(`
   - "mad"   → `>:(`

3. **Print and test:**  
   Call the function with various phrases and print the results.

```python
def emotify(sentence):
    # Step 2: Replace emotion words with emoticons
    sentence = sentence.replace("smile", ":)")
    sentence = sentence.replace("grin", ":D")
    sentence = sentence.replace("sad", ":(")
    sentence = sentence.replace("mad", ">:(")
    return sentence

# Step 3: Try it out!
print(emotify("Make me smile"))      # Output: 'Make me :)'
print(emotify("I am mad"))           # Output: 'I am >:('
print(emotify("What a grin"))        # Output: 'What a :D'
print(emotify("I am so sad"))        # Output: 'I am so :('
```

**Feel free to create your own sentences!**

---

## 3. 📦 Unpacking a List

**Goal:**  
Separate the first, middle, and last elements from a list.

### How does it work?

1. **Create a list:**  
   Example list: `[1, 2, 3, 4, 5, 6]`

2. **Extract elements:**
   - `first` gets the very first element (index `0`).
   - `middle` gets everything between the first and last (`1:-1`).
   - `last` gets the very last element (index `-1`).

3. **Print each part:**  
   Display them to see the separation.

```python
lst = [1, 2, 3, 4, 5, 6]

first = [lst[0]]      # Step 2a: First element
middle = lst[1:-1]    # Step 2b: All elements except first and last
last = [lst[-1]]      # Step 2c: Last element

# Step 3: Try it out!
print("first:", first)     # Output: first: [1]
print("middle:", middle)   # Output: middle: [2, 3, 4, 5]
print("last:", last)       # Output: last: [6]
```

**Try changing the list values or length, and see how the output changes!**

---

## 💡 Tips

- Play around! Change the function inputs and see the results.
- Add your own twists—what happens if you add more emoticons or use words in different cases?
- If you’re new to Python, try adding comments to explain each line in your own words.

---

Happy coding! 🚀  
