# Machine Learning

- a set of tools that allow us to teach computers how to perform tasks by providing examples of how they should be done.

1. **The Artificial Intelligence View**
- Learning is central to human knowledge and intelligence.
- Also essential for building intelligent machines.
- Automatic learning is crucial.

2. **THe Software Engineering View**
- ML allows us to program computers
- The use of learning tools to fine-tune or customize system performance in large-scale applications/systems will be more & more common.

3. **The Stats View**
- ML is the marriage of CS and Stats, the applicaion of computational techniques to stastical problems.
- Modern methods are concerned with learning models from large amounts of complex data, for which sophisticated models and fast algorithms are needed.

### Two Phases of Machine Learning Methods
1. **Training**: a model is learned from a collection of **training data**.
2. **Application**: the model is used to make decisions about some new **test data**.

### Main Types of Machine Learning
1. **Supervised Learning**: training data is labeled with the correct answers.
   - **classification**: outputs are discrete labels.
   - **regression**: outputs are real-valued
2. **Unsupervised Learning**: given a collection of unlabeled data, which we wish to analyze and discover patterns within.
   - **dimension reduction**
   - **clustering**
3. **Reinforcement Learning**
   - an agent (a robot or controller) seeks to learn the optimal actions to take based on the state of the world, and hence the consequences of past actions.

### Other Types of ML (most not covered in C11)
1. Semi-superivesed learning: a subset of the training data is labeled
2. Self-supervised learning: data are generated synthetically, often from real data, in a way that automatically generates labels.
3. Active Learning: obtaining data is expensive, so an algorithm must determine which training data to acquire.
4. Transfer/Meta/Few-Shot Learning: models learned from tasks with large training sets, or many tasks with moderate amounts of training data, can be used to help constrain learning on related problems that have relatively small datasets.
5. Strucutred Prediction: we learn models for complex structured objects, such as graphs or images, with many dimensions and complex dependencies among the predicted variables.
6. Time-series forecasting: used in financial markets
7. Anomaly detection: used for fault-detection in factories and in surveillance.

### Deep Learning
- predominant paradigm for ML and its widespread applications.
- refers to the use of `multi-layer neural networks` as a means of solving a spectrum of supervised and unsupervised ML problems.
- i.e. speech recognition and image classification
- exploded with emergence of Generative AI, use of the generative model for text data, computer code, speech signals, images, video, and audio.

### A simple 1D regression problem
- fit a 1D curve to a few points
- common to measure the quality of the fit in terms of the squared error between the given data and the fitted curve.
- The resulting fit from minimizing the squared error is called a `least-squares` estimate.
- When a model fits training data well, but performs poorly on test data, we say that the model has **overfit** the training data.
  - the model has fit properties of the input not paricularly relevant to the task at hand.
  - these properties are referred to as `noise`.
  - "the model does not generalize well to the test data" 
- ideally, we want a model that provides good predictions for new inputs
- often prefer simple, smooth models.
