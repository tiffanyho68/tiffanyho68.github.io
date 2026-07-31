# Projects

[Home](/) · [Projects](/projects) · [About](/about) · [Contact](/contact)

**Chat with an AI briefed on my work (Claude account required - free):** <a href="https://claude.ai/public/artifacts/fcfa0068-ffef-45a3-b08d-1c7ad3238622" target="_blank">Ask me anything</a>

## Cartoon Eyes Emotion Predictor
[GitHub](https://github.com/tiffanyho68/Cartoon-Eyes-Emotion-Predictor.git)

**The problem.** In my undergrad computer vision (CV) course, I built a model using a CNN to classify emotion from cartoon faces. In a later graduate CV course, I wanted to revisit it from a different angle: whether eyes alone - arguably the most expressive part of the face - could carry enough signal to classify emotions in cartoons, using a different method.

**What I did.** I switched from CNN to HOG feature extraction with an SVM classifier, and narrowed the input to eyes only. That constraint was deliberate: I wanted to isolate how much emotional signal the eyes carry on their own in cartoons, separate from the rest of the face.

**What came of it.** The model reached 55.56% accuracy - about 5% better than my original whole-face version, which surprised me; I expected eyes-only to be harder, not easier. The main failure was confusing angry with happy or sad, namely happy. Looking at the misclassifications, I think it comes down to how simplistic cartoon styles draw emotion: narrowed or squinted eyes show up for both anger and happiness, and in cartoons the mouth usually disambiguates the two - information an eyes only model doesn't have. I documented the full method, results, and limitations in a CHI format paper, with a clear next step: a larger, more diverse training set.

---

## Artificial Companionship Engagement
[GitHub](https://github.com/tiffanyho68/Artificial-Companionship-Engagement.git)

**The problem.** In a graduate human computer interactions (HCI) course, my group set out to study a modern phenomenon we'd all noticed and found significant: people becoming overly emotionally attached to AI companion chatbots, sometimes isolating from real relationships as a result. I wanted to combine a social issue with technical research - I've had my own experiences with mental health struggles and have always been drawn to understanding a range of mental health issues, so I proposed for us to investigate whether people with mental health struggles are more likely to form this kind of attachment.

**What I did.** My main role was research design: drafting the experiment questions and participant survey and writing the CHI format paper sections covering our literature review, methodology, and findings. A teammate built the chatbot itself, and I also contributed to the statistical testing for significance. We ran the study on classmates over a short data collection window, using a chatbot with customizable personality features, constrained by the budget available to us for more advanced tooling.

**What came of it.** We found only a slight positive correlation between mental health struggles and chatbot attachment - not statistically significant. Prior research (mostly in societies less open about mental health than the US) had shown a stronger positive correlation, which suggests our result may reflect real cultural difference as much as it reflects our study's limitations. Those limitations were real: a small, non-diverse participant pool (classmates only), academic time constraints on data collection, and budget limits on chatbot features. We concluded a larger, more diverse study over a longer window of time is needed to test this properly.

---

## Resume Classifier
[GitHub](https://github.com/tiffanyho68/Resume-Classifier.git) · [Video Demo](https://youtu.be/3YEI-1tER9Y)

**The problem.** In a graduate natural language processing (NLP) course, I could choose my own project topic. I was applying for internships at the time and thinking a lot about how companies filter applicants. Resumes aren't structured like typical documents, and I got curious whether I could build something similar to the systems companies actually use to screen resumes by keyword and predict job type.

**What I did.** I built a Naive Bayes classifier, a standard baseline for text classification and one I'd researched as a strong fit for the task, documenting the project in a YouTube video demo. For my data set, I pulled resumes from the internet across a variety of job types for training and testing.

**What came of it.** On a small test set of 6 resumes, the model got 4 correct. Looking at the misses, the real limitation wasn't the method - it was the data: too few job categories, too few resumes overall, and not enough variation within a single job type (e.g., two software engineer resumes can look very different, such as one leaning toward AI and the other toward cloud computing). A stronger version of this project would need a larger, more diverse resume set that also captures that kind of within category variation.

---

Seeking full-time AI/ML roles. If this kind of work is a fit for your team, I'd love to hear from you.

**[tiffanyho68@gmail.com](mailto:tiffanyho68@gmail.com)**
