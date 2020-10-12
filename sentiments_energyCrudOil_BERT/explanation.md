# Task to be performed:-

Using the `BERT` model to predicting kind of the sentiments
(in this case its truncated) of text in tweets about **energy crud
oil**. All of this can be achieved by using a `ktrain` wrapper.

## steps:-

* Splitting the dataset into training and test part.

* by using `text_from_df` method from `text` and providing necessary
parameters like:: `train_df`, `preprocess_mode`, `label_columns`, etc.
In return it gives vetors for `X_train`, `y_train`, `X_test`, `y_test` and
a preprocess mode is also returned.

* Next step is of creating a model by using `text_classifier` method from
`text`.

* Getting a learner for our model by using `get_learner`. This can be
usefull for getting a proper learning rate for particular use case. Also
this is for compiling the model.

* At last using the `get_predictor` method from `ktrain` predictions can be made.
