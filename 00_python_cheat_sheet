# 🐍 My Python Cheat Sheet

> **How to use this:** Don't read it top to bottom. `Ctrl+F` the thing you're
> trying to *do* ("filter", "unique", "group"). Organised by **what I want**,
> not by function name — because I never remember the function name.

---

## 🔍 Looking at data (first thing I do every time)

**See size + columns + a preview**
```python
df.shape        # (rows, columns)  -> no brackets, it's a property
df.columns      # the column names -> no brackets
df.head()       # first 5 rows     -> brackets, it's an action
df.info()       # columns + types + nulls, all at once
```

**Quick stats on the numbers**
```python
df.describe()   # count, mean, min, max, etc.
```

---

## ✂️ Grabbing columns by name pattern

**The skeleton I reuse for everything:**
```python
[ <output>  for <item> in <thing>  if <condition> ]
```

**All the ID columns**
```python
[c for c in df.columns if c.endswith('_id')]   # safer than 'id' in c
```

**All the score columns**
```python
score_cols = [c for c in df.columns if 'score' in c]
df[score_cols]                                 # select just those
```

---

## 🎯 Filtering rows

**Rows above a threshold**
```python
df[df['alert_score'] > 80]
```

**Rows matching a category**
```python
df[df['flag'] == 'high_risk']
```

---


```

---

## ⚠️ My personal gotchas (things I keep getting wrong)

| Mistake | Fix |
|---|---|
| `df.shape()` ❌ | `df.shape` — it's a property, no brackets |
| `df.head` ❌ (shows weird text) | `df.head()` — it's an action, needs brackets |
| `'id' in c` catches `valid`, `pyramid` | use `c.endswith('_id')` |
| `c in 'id' in c` | broken chain — just write `if 'id' in c` |

**Rule of thumb:** *Describing* the data = no brackets. *Doing something* to it = brackets.

---

## 📝 Add-your-own zone

_(paste anything here the moment you figure it out — future-you will thank you)_

-
-
-
