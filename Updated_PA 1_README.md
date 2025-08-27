# PA 1

## 1. ALPHABET SOUP PROBLEM

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

## 2. EMOTICON PROBLEM

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
---

## 3. UNPACKING LIST PROBLEM

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
