# Notes from Chapter 2
    - Bias Variance tradeoff --> This is a mathematical statement that no matter
      what your parameter model is, any attempt to decrease the bias by
      increasing flexibility will end up decreasing the variance. Moreover, bias
      and variance both contribute to the error term, so the tradeoff is in
      finding the right amount of flexibility that minimizes both bias and
      variance.

    - Bayes' classifier
        - This is a mathematical statement that when implementing a classifier
          model (e.g. predicting labels for Piazza posts), the classifier that
          minimizes the error term is the function: 
            P(Y = j | X = x_0), where x_0 is some input vector, and j is some
            state.
        In our example, the input vector would be the words used in the post,
        and the state would be the Piazza label attached to it.
        The Bayes' classifier then picks the label with the highest probability. 
    - KNN approach for a Bayes' classifier.
        - This idea is a simple idea that for predicting the Bayes' classifier,
          we just pick a point x_0, and then find the K-nearest neighbors (KNN)
          to that point. Then, estimate P(Y = j | X = x_0) by the proportion of
          points amongst the K neighbors that have value j. 
        - This turns out to work pretty well in practice
