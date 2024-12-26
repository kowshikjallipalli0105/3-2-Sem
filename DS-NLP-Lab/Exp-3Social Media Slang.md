# Demonstrate object standardization such as replace social media slangs from a text. 

## Steps:

### Create the dictionary

```
slang_dict={
    
    "lol":"Laugh Out Loud",
    "Omg":"Oh My God",
    "tq":"Thank You",
    "jk":"Just Kidding",
    "smh":"Shake My Hand",
    "afaik":"As Far As I know",
    "asap":"As Soon As Possible",
    "tbh":"To Be Honest",
    "idk":"I Don't Know",
    "imho":"In My Humble Opinion"
}
```
### creating the fuction code in which we use the dict

```
def st(text):
  words=text.split()
  standardized_words=[]
  for word in words:
    if word.lower() in slang_dict:
      standardized_words.append(slang_dict[word.lower()])
    else:
      standardized_words.append(word)
  return ''.join(standardized_words)
```

### calling the fuction

```
text="lol that's so tbh idk why imho they would do"
print(st(text))
```

### Output:
>text="lol that's so tbh idk why imho they would do"
print(st(text))
