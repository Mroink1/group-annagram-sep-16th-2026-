# group-annagram-sep-16th-2026-
notes: a LOT of functions were used here (most of (which I was a little confused on how they related to each other but that only piqued interest). I'm curious on how functions like "return", "values" work since they're so interesting to see collide. 

from collections import defaultdict

def group_anagrams(a):
    dfdict = defaultdict(list)
    for i in a:
        sorted_i = " ".join(sorted(i))
        dfdict[sorted_i].append(i)
    return dfdict.values()

words = ['tea', 'eat', 'ate']
print(group_anagrams(words))
