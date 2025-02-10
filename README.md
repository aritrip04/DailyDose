def sortsentence(s):
    words=s.split()
    n=len(words)
    original_words=[""]*n
    for i in words:
        position=int(i[-1])-1
        original_words[position]=i[:-1]
    return " ".join(original_words)
s1="is2 sentence4 This1 a3"
s2="Myself2 Me1 I4 and3"
print(sortsentence(s1))
print(sortsentence(s2))
