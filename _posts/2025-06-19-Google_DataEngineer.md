---
layout: post
title: Google_DataEngineer
permalink: /quizzes/google-dataengineer/
---



### 🧩 Problem

> Given an array of integers nums and an integer target...

### 💡 Thought Process

- Use a hashmap to check for complements...

### ✅ Solution (Python)

```python
def twoSum(nums, target):
    lookup = {}
    for i, num in enumerate(nums):
        if target - num in lookup:
            return [lookup[target - num], i]
        lookup[num] = i
