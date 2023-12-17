import string
def count_specific_words(text, specific_words):
    text = text.translate(str.maketrans('', '', string.punctuation)).lower()
    
    words = text.split()

    word_count = {word: 0 for word in specific_words}
    
    for word in words:
        if word in word_count:
            word_count[word] += 1
    
    return word_count

text = """
"""

woorden_neger = ["neger"]
woorden_positieve_associatie = ["lief","vrede","glimlach","hoop","dankbaarheid","succes","vriendschap","vrijheid","creativiteit","avontuur"]
woorden_negatieve_associatie = ["slecht","stom","afschuwelijk","ondraaglijk","vervelend","irritant","onaangenaam","onaantrekkelijk","verschrikkelijk","onbetrouwbaar"]

word_count_neger = count_specific_words(text, woorden_neger)
word_count_positive = count_specific_words(text, woorden_positieve_associatie)
word_count_negative = count_specific_words(text, woorden_negatieve_associatie)

for word, count in word_count_neger.items():
    print(f"Aantal keer '{word}' in tekst: {count}")
print()
for word, count in word_count_positive.items():
    print(f"Aantal keer '{word}' in tekst: {count}")
print()
for word, count in word_count_negative.items():
    print(f"Aantal keer '{word}' in tekst: {count}")
