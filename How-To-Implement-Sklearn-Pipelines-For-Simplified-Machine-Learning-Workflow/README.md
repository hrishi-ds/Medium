<img src="https://cdn-images-1.medium.com/max/1200/1*Eu3ck29Z0b51iXgEQ5pI-Q.png" width=1000 height=400>

<a href="https://github.com/hrishi-ds/Medium/tree/main/How-To-Implement-Sklearn-Pipelines-For-Simplified-Machine-Learning-Workflow">This notebook</a> contains the code used in my Medium story regarding how to use sklearn pipelines. 

## Why do we care about the pipelines?
### 1. It drastically simplifies our code
Instead of applying each step separately, we can now apply the pipeline to our data as a single large step. This will significantly reduce the amount of code and also make it more intuitive to understand.
### 2. It ensures the same pre-processing steps will also be applied to the test data
We must apply the same pre-processing steps used for our train set, onto our test set in the correct order. Having a pipeline of steps reduces the chance of incorrectly applying the steps to test data.
### 3. It allows to cross-validate the pre-processing steps (not just the model!) 
Typically, we only cross-validate our model, not the pre-processing workflow. But with the pipeline, we can easily cross-validate the steps and hence also optimize them as necessary.
### 4. Finally, it reduces the risk of data leakage.
Data leakage occurs when our ML model accidentally sees👀 the test data. And therefore having a pipeline ensures that the relevant method is being applied to the correct subset of data.
