## this Roadmap is provided by Reddit user MarcelDeSutter

# Introduction

As announced I extend this guide with some remarks.

I myself am a trained business psychologist, so I had little connection to ML during my undergrad studies. My fascination for this technology arose quite late, which is why I enrolled at a technical university again a year ago to learn the basics of computer science. Most of my knowledge, however, I have taught myself in self-study and in the following I will break down my main insights.

I think there are three basic areas that should be covered if you want to be a competent ML engineer: mathematics, concrete ML knowledge and programming skills. These are rough categories and I don't want to give the impression that this is all there is to it, but I notice the biggest progress in myself when I practice all three areas regularly over a longer period of time. I recommend that anyone who wants to learn ML professionally should take all three areas equally seriously and to study them simultaneously if possible.

# Mathematics

Not all areas of mathematics are relevant to ML. The ones that are most important to ML are Linear Algebra, Probability Theory and Multivariable Calculus, for which there are a lot of good online courses. Some of them I've listed below.

We need linear algebra because the data we deal with in ML contexts are stored in n-dimensional arrays. An understanding of the interplay between scalars, vectors, matrices and tensors is therefore essential for everything we hope to do with our data. Linear Algebra will be the language we will be speaking when doing ML of any kind.

We often need probability theory to explain why a particular learning algorithm works, where certain cost functions come from, and so on. Often it is about maximizing probabilities, which cannot be understood without an understanding of basic stochastic concepts.

Everywhere in the ML context we encounter multidimensional functions and the confident handling of them is necessary to understand how our algorithms work. If there are no closed form solutions for the optimal parameters of a learning algorithm, for example, iterative methods are often used to learn the parameters. In this case, the gradient of a cost function is often used, which is obtained from the partial derivatives of a multidimensional function.

For general intuition, I think 3Blue1Brown is the best place to start:

Linear Algebra: [https://www.youtube.com/watch?v=fNk\_zzaMoSs&list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE\_ab](https://www.youtube.com/watch?v=fNk_zzaMoSs&list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)

Calculus: [https://www.youtube.com/watch?v=WUvTyaaNkzM&list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr](https://www.youtube.com/watch?v=WUvTyaaNkzM&list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)

After you've got the intuition and refreshed the basics of high school mathematics, I can recommend the following more in-depth courses:

Probability Theory: [https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-041sc-probabilistic-systems-analysis-and-applied-probability-fall-2013/](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-041sc-probabilistic-systems-analysis-and-applied-probability-fall-2013/) This is HANDS-DOWN the best course I've ever taken. I found the content very difficult, probably due to my non-mathematical background, but I still have the feeling that I came out of the course with a deep understanding of probability theory. Some of the content you will probably hardly see again in ML contexts, but the basic concepts like counting, conditional probabilities, random variables, distribution functions, MLE and MAP, Bayesian Inference, etc. are extremely well explained.

Linear Algebra: [https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/](https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/) Gilbert Strang is just a gangster in Linear Algebra. I love his lecture style and he manages to make linear algebra super tangible.

Calculus I-III: [https://www.youtube.com/user/amarchese22/playlists?disable\_polymer=1](https://www.youtube.com/user/amarchese22/playlists?disable_polymer=1) I just got this playlist recommended two days ago, but the many visualizations and digestible video lengths seem to be good conditions for a good information transfer. I suggest to at least check out Calculus I and II.

Multivariable Calculus: [https://www.youtube.com/playlist?list=PLSQl0a2vh4HC5feHa6Rc5c0wbRTx56nF7](https://www.youtube.com/playlist?list=PLSQl0a2vh4HC5feHa6Rc5c0wbRTx56nF7) Here is again 3Blue1Brown with his amazing video series on multivariable Calculus. I think this playlist has exactly the right depth, not too trivial, but also not unnecessarily packed with abstract proofs. There are certainly more complex and deeper courses for multivariable Calculus, but for prospective ML Engineers this is more than appropriate.

Matrix Methods: [https://ocw.mit.edu/courses/mathematics/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/](https://ocw.mit.edu/courses/mathematics/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/) Another course by Gilbert Strang. There all three areas (linear algebra, probability theory, multivariable calculus) are combined with applications in ML.

After these courses there should be little mathematics that will surprise you later.

# Concrete ML Knowledge

Andrew Ng has, in my opinion, taken the undisputed position of offering the world the Holy Trinity of basic ML education. Everything builds on each other and is more practice-oriented than it is theoretical. Although mathematical notation is used, everything is still comparatively basic.

Andrew Ng's ML course: [https://www.coursera.org/learn/machine-learning](https://www.coursera.org/learn/machine-learning) Even though the course may seem very demanding (I've needed three attempts) at first, you'll remember him forever as Prof Ng explains the basics of ML like hardly anyone else. However, the course shows its age because MATLAB is not a language that is up-to-date for ML. When working on the code assignments, you should therefore google for Python implementations and work on them instead.

The other two courses are the logical continuation of Andrew Ng's first ML course.

Andrew Ng's Deep Learning Specialization: [https://de.coursera.org/specializations/deep-learning](https://de.coursera.org/specializations/deep-learning)

Andrew Ng's Tensorflow in Practice Specialization: [https://de.coursera.org/specializations/tensorflow-in-practice](https://de.coursera.org/specializations/tensorflow-in-practice)

After that you are ready for advanced courses:

Old but gold, the CS229 lectures of 2008: [https://www.youtube.com/watch?v=UzxYlbK2c7E&list=PLA89DCFA6ADACE599](https://www.youtube.com/watch?v=UzxYlbK2c7E&list=PLA89DCFA6ADACE599) This is Ng's coursera ML course on steroids. Have you wondered why logistic regression uses the sigmoid function? Here you will find the answer. Have you always wanted to know how to derive the Normal Equation? Here you will find the answer. The course is sometimes bashed on the fact that it is old, but the reality is that the concepts presented here also work in the age of neural networks and are sometimes even preferable. Classical models just do their job well, too.

And a modern rendition: [https://www.youtube.com/watch?v=vT1JzLTH4G4&list=PLa-Bt050gYuhEeLRG8YBmFxwLvTJ5FqPS](https://www.youtube.com/watch?v=vT1JzLTH4G4&list=PLa-Bt050gYuhEeLRG8YBmFxwLvTJ5FqPS) Any criticism of the above course is nullified, as there is a current version of it. The focus here is more on neural networks, but that's why the old CS229 course is not outclassed.

I also like this set of online lectures: [http://www.cs.cornell.edu/courses/cs4780/2018fa/lectures/](http://www.cs.cornell.edu/courses/cs4780/2018fa/lectures/) Somehow I always come across these lectures while doing my own research. I think they are very good and the focus is rather probabilistic. The only catch, in my opinion, is that the lecturer's handwriting is very bad, which is why I always have the handout open in parallel. His accent is also funny.

# Programming Skills

Here I had to start from zero but I learned a lot in my complementary computer science studies, so I can't recommend as many resources as in the other sections. But when studying Python, I refered to Corey Schafer a lot, who has many wonderful Python tutorials on Youtube: [https://www.youtube.com/user/schafer5/playlists](https://www.youtube.com/user/schafer5/playlists)

There are also two books that I can recommend for learning Python, especially for ML and Data Science applications:

[https://jakevdp.github.io/PythonDataScienceHandbook/](https://jakevdp.github.io/PythonDataScienceHandbook/) It contains all important information about the packages NumPy, Pandas and Matplotlib, which are all used again and again when you want to program ML algorithms or prepare and visualize the necessary data.

[https://github.com/ageron/handson-ml](https://github.com/ageron/handson-ml) Please buy the paperback, the author deserves it. This book is the best application-oriented resource I know. I often find myself referring to this book.

Always try to implement the knowledge directly, i.e. to reprogram algorithms in Python. If that's too hard, google the code and try to understand it, we all do. Get familiar with the Scikit-Learn library and Tensorflow and try to complete small projects that you can upload to Github. You won't get any better without practice. Learn app and web development to embed your projects into applications that are actually profitable for users.
