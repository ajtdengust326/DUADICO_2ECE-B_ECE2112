# PROBLEM ASSESSMENT 1

## 1. ALPHABET SOUP PROBLEM

**Goal:**  
My goal here was to rearrange the letters of a word in alphabetical order.

### How did I approach it?

1. **Define a function:**  
   I created a function named `alphabet_soup` that takes a word (string) as input.

2. **Sort the letters:**  
   I used Python’s built-in `sorted()` function to alphabetize the letters in the word.

3. **Join the letters back together:**  
  Since `sorted()` gives me a list, I used `''.join()` to turn it back into a string.

4. **Print the result:**  
  I called the function with my word and printed the result.

```python
def alphabet_soup(word):
                                      # Step 2 & 3: Sort and join the letters
    return "".join(sorted(word))

                                      # Step 4:
print(alphabet_soup("hello"))         # Output: 'ehllo'
print(alphabet_soup("hacker"))        # Output: 'acehkr'
```

## 2. EMOTICON PROBLEM

**Goal:**  
I wanted to automatically replace emotion words in a sentence with their emoticons.

### How did mkae it work?

1. **Define a function:**  
   I created a function named `emotify` that takes a sentence as input.

2. **Replace words with emoticons:**  
   I used `.replace()` to swap out emotion words for emoticons:
   - "smile" → `:)`
   - "grin"  → `:D`
   - "sad"   → `:(`
   - "mad"   → `>:(`

3. **Print and test:**  
   I called the function with various phrases and printed the results.

```python
def emotify(sentence):
                                               # Step 2: Replace emotion words with emoticons
    e = e.replace("smile", ":)")
    e = e.replace("grin", ":D")
    e = e.replace("sad", ":(")
    e = e.replace("mad", ">:(")
    return e

                                     # Step 3:
print(emotify("Make me smile"))      # Output: 'Make me :)'
print(emotify("I am mad"))           # Output: 'I am >:('
print(emotify("What a grin"))        # Output: 'What a :D'
print(emotify("I am so sad"))        # Output: 'I am so :('
```
---

## 3. UNPACKING LIST PROBLEM

**Goal:**  
I wanted to separate the first, middle, and last elements from a list.

### How did I do it to make it work?

1. **Create a list:**  
   Example list: `[1, 2, 3, 4, 5, 6]`

2. **Extract elements:**
   - I assigned `first` to the very first element (index `0`).
   - I assigned `middle` to everything between the first and last (`1:-1`). *The colon is used to slice the last element (-1) from the middle*
   - I assigned `last` to the very last element (index `-1`).
   
3. **Print each part:**  
   I displayed them to see the separation.

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
