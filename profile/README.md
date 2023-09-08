# The Harmony Project

Harmony is a tool using AI which allows you to compare items from questionnaires and identify similar content. You can try Harmony at https://app.harmonydata.org and you can read our blog at https://harmonydata.org/blog/.

The source code for Harmony is on Github at https://github.com/harmonydata/harmony.

[![Harmonising questionnaires](/profile/video.jpg)](https://www.youtube.com/watch?v=cEZppTBj1NI "Harmonising questionnaires")

## Harmonising Mental Health Data

Harmony is a data harmonisation project that uses Natural Language Processing to help researchers make better use of existing data from different studies by supporting them with the harmonisation of various measures and items used in different studies.

## Who worked on Harmony?

Harmony is a collaboration project between the University of Ulster, University College London, the Universidade Federal de Santa Maria in Brazil, and Fast Data Science Ltd.

The team at Harmony is made up of:

* Bettina Moltrecht, PhD (UCL)
* Dr Eoin McElroy (University of Ulster)
* Dr George Ploubidis (UCL)
* Dr Mauricio Scopel Hoffman (Universidade Federal de Santa Maria, Brazil)
* Thomas Wood ([Fast Data Science](https://fastdatascience.com))

## Who to contact about Harmony?

You can contact us at https://harmonydata.org/contact/.

## How do I cite Harmony?

McElroy, E., Moltrecht, B., Ploubidis, G.B., Scopel Hoffman, M., Wood, T.A., Harmony [Computer software], Version 1.0, accessed at https://app.harmonydata.org. Ulster University (2022)

## Does Harmony store my data?

If you upload a questionnaire or instrument, Harmony does not store or save it. You can read more on our [Privacy Policy page](https://harmonydata.org/privacy-policy/).

## How does Harmony work?

Harmony passes the text of each questionnaire item through a neural network called Sentence-BERT, in order to convert it into a vector. The similarity of two texts is then measured as the similarity between their vectors. Two identical texts have a similarity of 100% while two completely different texts have a similarity of 0%. You can read more in this [technical blog post](https://harmonydata.org/how-does-harmony-work/) and you can even [download and run Harmony’s source code](https://github.com/harmonydata/harmony).

## How reliable is Harmony?

Harmony was able to reconstruct the matches of the questionnaire harmonisation tool developed by McElroy et al in 2020 with the following AUC scores: childhood 81%, adulthood 77%. Harmony was able to match the questions of the English and Portuguese GAD-7 instruments with AUC 100%. You can read more in [this blog post](https://harmonydata.org/measuring-the-performance-of-nlp-algorithms/).

## What do the numbers mean?

The numbers are the cosine similarity of document vectors. The cosine similarity of two vectors can range from -1 to 1 based on the angle between the two vectors being compared. We have converted these to percentages. We have also used a preprocessing stage to convert positive sentences to negative and vice-versa (e.g. I feel anxious -> I do not feel anxious). If the match between two sentences improves once this preprocessing has been applied, then the items are assigned a negative similarity.

## Does Harmony give p-values?
At this time Harmony does not give p-values. But you can interpret the percentage matches like correlation coefficients. In future we hope to provide more statistical data to Harmony’s users.

## Who developed the Python code of Harmony?

* Thomas Wood ([Fast Data Science](https://fastdatascience.com))
