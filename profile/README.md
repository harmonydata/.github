![The Harmony Project logo](https://raw.githubusercontent.com/harmonydata/brand/main/Logo/PNG/%D0%BB%D0%BE%D0%B3%D0%BE%20%D1%84%D1%83%D0%BB-05.png)

<a href="https://harmonydata.ac.uk"><span align="left">🌐 harmonydata.ac.uk</span></a>
<a href="https://www.linkedin.com/company/harmonydata"><img align="left" src="https://raw.githubusercontent.com//harmonydata/.github/main/profile/linkedin.svg" alt="Harmony | LinkedIn" width="21px"/></a>
<a href="https://twitter.com/harmony_data"><img align="left" src="https://raw.githubusercontent.com//harmonydata/.github/main/profile/x.svg" alt="Harmony | X" width="21px"/></a>
<a href="https://www.instagram.com/harmonydata/"><img align="left" src="https://raw.githubusercontent.com//harmonydata/.github/main/profile/instagram.svg" alt="Harmony | Instagram" width="21px"/></a>
<a href="https://www.facebook.com/people/Harmony-Project/100086772661697/"><img align="left" src="https://raw.githubusercontent.com//harmonydata/.github/main/profile/fb.svg" alt="Harmony | Facebook" width="21px"/></a>
<a href="https://www.youtube.com/channel/UCraLlfBr0jXwap41oQ763OQ"><img align="left" src="https://raw.githubusercontent.com//harmonydata/.github/main/profile/yt.svg" alt="Harmony | YouTube" width="21px"/></a>

💁You can run the walkthrough notebook in [Google Colab](https://colab.research.google.com/github/harmonydata/harmony/blob/main/Harmony_example_walkthrough.ipynb) with a single click: <a href="https://colab.research.google.com/github/harmonydata/harmony/blob/main/Harmony_example_walkthrough.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

Here is an [example R notebook in R markdown](https://harmonydata.ac.uk/harmony_r_example.nb.html).

# The Harmony Project

Harmony is a tool using AI which allows you to compare items from questionnaires and identify similar content. You can try Harmony at https://app.harmonydata.ac.uk and you can read our blog at https://harmonydata.ac.uk/blog/.

The source code for Harmony is on Github at https://github.com/harmonydata/harmony.

[![Harmonising questionnaires](/profile/video.jpg)](https://www.youtube.com/watch?v=cEZppTBj1NI "Harmonising questionnaires")

# Looking for source code?

* 🖱️ The Harmony app which is running at https://harmonydata.ac.uk/app is in this repo: https://github.com/harmonydata/app.
* 👨‍💻 The Harmony Python library source code is here: https://github.com/harmonydata/harmony.
* 🇷 The Harmony R library source code is here: https://github.com/harmonydata/harmony_r.
* 💻 The Harmony API source code is here: https://github.com/harmonydata/harmonyapi.
* 📔 Finally, the source code of the Harmony static blog at https://harmonydata.ac.uk is in this repo: https://github.com/harmonydata/harmonydata.github.io. It is hosted with [Github Pages](https://pages.github.com/).

## 💚 Harmonising Mental Health Data

The Harmony project is a data harmonisation project that uses [Natural Language Processing](https://fastdatascience.com/guide-natural-language-processing-nlp/) to help researchers make better use of existing data from different studies by supporting them with the harmonisation of various measures and items used in different studies.

## ‎😃💁Who worked on Harmony?

Harmony is a collaboration project between [Ulster University](https://ulster.ac.uk/), [University College London](https://ucl.ac.uk/), the [Universidade Federal de Santa Maria](https://www.ufsm.br/), and [Fast Data Science](http://fastdatascience.com/).  Harmony is funded by [Wellcome](https://wellcome.org/) as part of the [Wellcome Data Prize in Mental Health](https://wellcome.org/grant-funding/schemes/wellcome-mental-health-data-prize).

The team at Harmony is made up of:

* Bettina Moltrecht, PhD (UCL)
* Dr Eoin McElroy (University of Ulster)
* Dr George Ploubidis (UCL)
* Dr Mauricio Scopel Hoffman (Universidade Federal de Santa Maria, Brazil)
* Thomas Wood ([Fast Data Science](https://fastdatascience.com))

## ✉️Who to contact about Harmony?

You can contact us at https://harmonydata.ac.uk/contact/.

## 📜How do I cite Harmony?

McElroy, E., Moltrecht, B., Ploubidis, G.B., Scopel Hoffman, M., Wood, T.A., Harmony [Computer software], Version 1.0, accessed at https://app.harmonydata.ac.uk. Ulster University (2022)

## 🔢Does Harmony store my data?

If you upload a questionnaire or instrument, Harmony does not store or save it. You can read more on our [Privacy Policy page](https://harmonydata.ac.uk/privacy-policy/).

## ⚙️How does Harmony work?

Harmony passes the text of each questionnaire item through a neural network called Sentence-BERT, in order to convert it into a vector. The similarity of two texts is then measured as the similarity between their vectors. Two identical texts have a similarity of 100% while two completely different texts have a similarity of 0%. You can read more in this [technical blog post](https://harmonydata.ac.uk/how-does-harmony-work/) and you can even [download and run Harmony’s source code](https://github.com/harmonydata/harmony).

## 🎯How reliable is Harmony?

Harmony was able to reconstruct the matches of the questionnaire harmonisation tool developed by McElroy et al in 2020 with the following AUC scores: childhood 81%, adulthood 77%. Harmony was able to match the questions of the English and Portuguese GAD-7 instruments with AUC 100%. You can read more in [this blog post](https://harmonydata.ac.uk/measuring-the-performance-of-nlp-algorithms/).

## 🧮What do the numbers mean?

The numbers are the cosine similarity of document vectors. The cosine similarity of two vectors can range from -1 to 1 based on the angle between the two vectors being compared. We have converted these to percentages. We have also used a preprocessing stage to convert positive sentences to negative and vice-versa (e.g. I feel anxious -> I do not feel anxious). If the match between two sentences improves once this preprocessing has been applied, then the items are assigned a negative similarity.

## 📊 Does Harmony give p-values?
At this time Harmony does not give p-values. But you can interpret the percentage matches like correlation coefficients. In future we hope to provide more statistical data to Harmony’s users.

## 🧑 Who developed the Python code of Harmony?

* Thomas Wood ([Fast Data Science](https://fastdatascience.com))
