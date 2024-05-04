# Pick-Pulsar-Classifier

Pulsars are important objects of astronomical study. From our telescopes, they appear as relatively periodical pulses of radiation bursts.  Due ot various factors, such as how weak the signals usually are, and how artificial signals may interfere with them, pulsar detection is often difficult and time consuming for astronomers. Most pulsar candidates examined by astronomers turn out to not be pulsars, which leads to wasted time and money for astronomers.

Learning algorithms may offer a way to speed this process and reduce the amount of human labor required. Supervised Learning Algorithms are a subcategory of learning algorithms defined by the use of labeled data to train a classifier model. Input data is fed to the model, consisting of a set of parameters, or attributes, and a label. The algorithm adjusts the weights attributed to each parameter until the model is fit appropriately. This model can be used to classify the objects of new datasets. Astronomy has collected various unbalanced datasets on pulsar candidates, that have already been classified by human astronomers. This study aims to assess whether supervised learning models trained on these datasets could be effective enough at classifying previously unseen objects as either pulsars or not pulsars, to aid in astronomical research.

The project studies the best samplers to balance the unbalanced training dataset of identified pulsars and false pulsar candidates, and compares the performance of various classifiers, trained in such balanced dataset, when classifying both balanced and unbalanced test sets.


