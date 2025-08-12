---
layout: default
title: "Counting sort"
date: 2025-08-11
description: "///"
---

```cpp
vector<int> cnt(10, 0);

for (auto el: a)
    ++cnt[el];
a.resize(0);

for (int i= 0; i < cnt.size(); ++i)
    a.insert(a.end(), cnt[i], i);
```
