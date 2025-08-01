# Improving Model Quality With TensorFlow Model Analysis

## Introduction

As you tweak your model during development, you need to check whether your
changes are improving your model. Just checking accuracy may not be enough. For
example, if you have a classifier for a problem in which 95% of your instances
are positive, you may be able to improve accuracy by simply always predicting
positive, but you won't have a very robust classifier.

## Overview

The goal of TensorFlow Model Analysis is to provide a mechanism for model
evaluation in TFX. TensorFlow Model Analysis allows you to perform model
evaluations in the TFX pipeline, and view resultant metrics and plots in a
Jupyter notebook. Specifically, it can provide:

*   [Metrics](https://tensorflow.github.io/model-analysis/metrics) computed on entire training and holdout
    dataset, as well as next-day evaluations
*   Tracking metrics over time
*   Model quality performance on different feature slices
*   [Model validation](https://tensorflow.github.io/model-analysis/model_validations) for ensuring that
    model's maintain consistent performance

## Next Steps

Try our [TFMA tutorial](https://tensorflow.github.io/tfx/tutorials/model_analysis/tfma_basic).

Check out our [github](https://github.com/tensorflow/model-analysis) page for
details on the supported
[metrics and plots](https://tensorflow.github.io/model-analysis/metrics) and associated notebook
[visualizations](https://tensorflow.github.io/model-analysis/visualizations).

See the [installation](https://tensorflow.github.io/model-analysis/install) and
[getting started](https://tensorflow.github.io/model-analysis/get_started) guides for information and
examples on how to get [set up](https://tensorflow.github.io/model-analysis/setup) in a standalone
pipeline. Recall that TFMA is also used within the [Evaluator](evaluator.md)
component in TFX, so these resources will be useful for getting started in TFX
as well.
