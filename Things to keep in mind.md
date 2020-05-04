### Things to keep in mind
1. Randomly shuffle the data before using - this is to avoid accidently introducing ordering in the training data
2. Respect arrow of time - If predicting future using past data, do not change ordering of data! Training data should be in past
3. Remove redundancy in data - Training and validation sets should be disjoint

### Data pre-processing general steps
1. Vectorize the data before using
2. Value normalization - this helps avoid converging faster
3. Handle missing values - in general, using 0 to represent missing data helps, this is if 0 doesn't have a meaning in itself. Neural networks learns to ignore it. If only test data has the missing data, try introducing the examples in training process too ( even if artificially generate )

### Feature engineering
1. Requires understanding problem in depth!
