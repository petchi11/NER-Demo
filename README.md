# NER-Demo

## PROGRAM 
```python
import spacy
from spacy import displacy

nlp = spacy.load('en_core_web_sm')

nlp.pipe_names

doc = nlp("Petchi Mani is Living in TamilNadu.")

for ent in doc.ents:
  print(ent.text," - ", ent.label_, " - ", spacy.explain(ent.label_))
  
displacy.render(doc, style="ent", jupyter=True)

```
