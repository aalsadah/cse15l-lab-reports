## Four GREP Command-line Options
**1.**
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

**2.**
```grep -v``` This command inverts the search, so if you do a search for the letter "i" you will get every line that does **not** contain an i. I found this information on [Wikibooks](https://en.wikibooks.org/wiki/Grep)
```
-bash-4.2$ grep -v "i" journal.pbio.0020001.txt











        2002).


            Canada?




        programs.


        journals (
        Nature and
        to the top 11–20 journals.
        In


        A Long Road Yet to Travel
        world.






```
```
-bash-4.2$ grep -v "celiac" pmed.0010023.txt





        adherence to a gluten-free diet. This means no wheat, rye, barley, and, until recently, no
        oats. Then some recent studies suggested that oats did not cause the intestinal
        inflammation characteristic of the disease, and thus oats are now often included in the
        they can and must not eat, but a study by Ludvig Sollid and colleagues in this issue of
        PLoS Medicine suggests that oats are not safe in all cases.
        interplay between genetic and environmental factors, but it is better understood than most.
        Long believed to be a relatively rare disorder, it is now thought to affect about one in
        250 people worldwide. Clinical symptoms are present in less than half of patients and vary
        considerably. Genetically, almost all patients have one of two predisposing HLA molecules,
        which determine the context in which their immune system encounters foreign antigens,
        disease, the immune system mounts an abnormal response to gluten, which is characterized by
        gluten-reactive intestinal T cells and by inflammation and compromised function of the
        small intestine.
        range of molecular pathology tools to studying the response to oats of nine patients with
        oats, and four of them had shown clinical symptoms after oats ingestion. The goal of the
        study was to characterize the intestinal T cell response to oats in these patients, and to
        relate it to clinical symptoms and intestinal biopsy results. All patients were on a
        gluten-free diet and ate oats that were free of contamination by other cereals.
        Three of the four patients who had reported problems after eating oats showed intestinal
        cells from these three patients. Two of the five patients who seemed to tolerate oats also
        had oats-reactive intestinal T cells. Functional study of these T cells showed that they
        peptides derived from oat avenin that are very similar to peptides of gluten.
        Taken together, the findings show that intolerance to oats exists at least in some
        oats that other patients have to wheat, barley, or rye. However, identical reactions were
        also seen in two of the patients who were clinically tolerant to oats. The authors suggest
        that these reactions could develop into symptomatic disease after some time delay, but
        there is no proof that the presence of oats-reactive T cells is an indicator of future
        symptoms or even of enhanced susceptibility to clinical oats intolerance.
        determine the frequency of oats intolerance.


```

**3.**
```grep -c``` This command gives you a count of the matching lines, which is helpful if you want to know the number of matching lines. I found this information on [Wikibooks](https://en.wikibooks.org/wiki/Grep)

```
-bash-4.2$ grep -c "celiac" pmed.0010023.txt
10
```
```
-bash-4.2$ grep -c "a" journal.pbio.0020001.txt
196
```
**4.** 
```grep -n``` This command is similar to ```grep -c``` but it gives adds each matching line's line number before it, this can be very helpful in giving you the location of the thing you are searching for in the file being searched. I found this information on [Wikibooks](https://en.wikibooks.org/wiki/Grep)
```
-bash-4.2$ grep -n "celiac" pmed.0010023.txt
6:        Most patients with (celiac) disease can eliminate their symptoms—at a price: life-long
10:        (celiac) disease diet. This is good news for patients coping with severe restrictions on what
13:        Like other chronic inflammatory diseases, (celiac) disease is caused by a complex
19:        including gluten proteins found in wheat and other cereals. In individuals with (celiac)
23:        Ludvig Sollid and colleagues applied the current understanding of (celiac) disease and a
25:        (celiac) disease. The nine patients were not a random sample: all of them had been eating
31:        inflammation typical of (celiac) disease, and Sollid and colleagues studied intestinal T
34:        were restricted to (celiac)-disease-associated HLA molecules and that they recognized two
37:        patients with (celiac) disease, and that those patients have the same molecular reaction to
43:        Oats are not safe for all patients with (celiac) disease, but future studies are needed to
```
```
-bash-4.2$ grep -n "molecular" pmed.0010023.txt
24:        range of (molecular) pathology tools to studying the response to oats of nine patients with
37:        patients with celiac disease, and that those patients have the same (molecular) reaction to
```
