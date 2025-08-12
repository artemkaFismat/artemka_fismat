---
layout: default
title: "Merge sort"
date: 2025-08-11
description: "///"
---
```cpp
vector<int> merge(vector<int> a, vector<int> b) {
    vector<int> res;
    int i = 0;
    int j = 0;
    while (i < a.size() && j < b.size()) {
        if (a[i] <= b[j])
            res.push_back(a[i++]);
        else
           res.push_back(b[j++]);
    }
    while (i < a.size())
        res.push_back(a[i++]);
    while (j < b.size())
        res.push_back(b[j++]);
    return res;
}
vector<int> msort(vector<int> a) {
    if (a.size() <= 1)
        return a;
    int k = a.size() / 2;
    return merge(
        msort(vector<int>(a.begin(), a.begin() + k)),
        msort(vector<int>(a.begin() + k, a.end())));
}
```
