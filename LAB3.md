## Four GREP Command-line Options

```grep -i``` This command line option ignores lowercase and uppercase. You can see in the second example that the search for the world "clinical", shows the word "Clinical" with the only diffrence being upper vs lower case. -i can be useful if you do not care about the case of a word and are just looking for it. I found this information on [Wikibooks](https://en.wikibooks.org/wiki/Grep)
``` 
-bash-4.2$ grep -i "celiac" pmed.0010023.txt
        Most patients with (celiac) disease can eliminate their symptoms—at a price: life-long
        (celiac) disease diet. This is good news for patients coping with severe restrictions on what
        Like other chronic inflammatory diseases, (celiac) disease is caused by a complex
        including gluten proteins found in wheat and other cereals. In individuals with (celiac)
        Ludvig Sollid and colleagues applied the current understanding of (celiac) disease and a
        (celiac) disease. The nine patients were not a random sample: all of them had been eating
        inflammation typical of (celiac) disease, and Sollid and colleagues studied intestinal T
        were restricted to (celiac)-disease-associated HLA molecules and that they recognized two
        patients with (celiac) disease, and that those patients have the same molecular reaction to
        Oats are not safe for all patients with (celiac) disease, but future studies are needed to
```
```
-bash-4.2$ grep -i "clinical" pmed.0010023.txt
        250 people worldwide. (Clinical) symptoms are present in less than half of patients and vary
        oats, and four of them had shown (clinical) symptoms after oats ingestion. The goal of the
        relate it to (clinical) symptoms and intestinal biopsy results. All patients were on a
        also seen in two of the patients who were (clinical)ly tolerant to oats. The authors suggest
        symptoms or even of enhanced susceptibility to (clinical) oats intolerance.
```

