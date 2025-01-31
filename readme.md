Name: Lance Belen

Instructions to execute the script file:

1. Ensure that the files Assignment2.ipynb, avila-tr.csv, and avila-ts.csv are in the same directory.
2. Launch Jupyter Notebook and open Assignment2.ipynb.
3. On the top menu, click Kernel, then click Restart Kernel and Run All Cells...

<h1>ABSTRACT / EXECUTIVE SUMMARY</h1>h1>
The Avila Bible case consists of a dataset that has been created from 800 images of the
Abila Bible. The Avila Bible is a giant Latin copy of the whole Bible from the 12th century
(Stefano, Fontanella, Maniaci, Freca, 2018). Manuscript studies showcase different methods
and techniques of analysis that are applicable in different areas of the industry (Herman,
Ransom, 2023). Here, this is utilised for the purpose of exploring the world of computing
technology through a core step in data science. The Avila Bible Case is the study of
standardised handwriting and book typology that dives into the analysis of basic layout
features, page organisation, and exploitation of available space which provides significant
findings that can be used to develop a predictive system that will identify the scribes who
worked together to write the Avila Bible. This report will go through the data science process
that I have implemented using the Avila Bible Case dataset to focus on data modelling which is
a core step in the data science process. This is intended to gain practical knowledge
of the steps of data modelling, presentation, and automation. The data is first retrieved and
prepared for exploration through data preprocessing. Then, it is modelled through two
supervised machine-learning methods that fall under the category of classification. I used two
different methods for modelling, namely the K-Nearest Neighbour method and the Decision
Tree method. Finally, the evaluation of these models is done through K-Fold Cross Validation to
confirm and compare the effectiveness of the two models in predicting/identifying the scribes
given a set of trained typological features/data against the test set.

<h1>INTRODUCTION</h1>
The core step of the data science process is data modelling. This allows the
communication or representation of connections between data points and structure (IBM,
2024). Through this, a system can be created to predict an outcome by providing a set of
trained data of features that correspond to actual results. In this case, the scribes are the
“results” of 10 typological features that can be used by the model to analyse and learn the
traits of each scribe’s handwriting and distinguish each of their characteristics in terms of the
medieval scripting of the Avila Bible. The two Classification models, built through the
K-Nearest Neighbour method and the Decision Tree method, I was able to reach the goal of the
project, which is to develop a scribe recognition system that, to an extent, accurately predicts
the scribe given a set of test data.

Before data modelling, I first performed data retrieval and preprocessing which did not
require much more cleaning as the dataset, as per Stefano, Fontanella, Maniaci, and Freca, in
2018, the authors of the report “Reliable Writer Identification in medieval manuscripts through
page layout features: The ‘‘Avila’’ Bible case”, has already been normalized by using the
Z-normalization method. Given that the normalisation of data is for the removal of a possible
unorganised nature and redundancy to allow a standardised dataset, I still handled the outliers
and checked for missing values to serve as a second layer of data preparation to reach a closer
chance of predictive accuracy for the model.

Following preprocessing, I explored the data to further provide an identication of
possible inaccuracies or errors and hence, handle these again accordingly. However, the data
exploration is mainly to observe how the features in the dataset are depicted and the
characteristics or nature that each holds, as well as the relationships between pairs of selected
features to reach a plausible hypothesis for the target variable. The features have been
separated into three categories; Set 1 is for highlighting chronological and/or typological
differences; related to the geometrical properties of the page, set 2 is mainly concerned with
the exploitation of each column of the written area, and set 3 provides the characteristics of
the scribe in terms of text distribution per row. That being said, the exploration of each of the
features are separated into the same three categories as well to individually address the
observations that provide signification information accordingly.

The specific categorization of the features:
Set 1 - Intercolumnar distance, Upper margin, Lower Margin
Set 2 - Exploitation, Row number, Modular ratio, Interlinear spacing
Set 3 - Weight, Peak number, Modular ratio/Interlinear spacing

Finally, as mentioned already, data modelling is the last task of this assignment which I
performed through the methods K-Nearest Neighbour and Decision Tree, both of which are a
Classification method of modelling. The data set has actually already been separated into two
sets, the train and test set, so I just re-established these sets of data after the necessary
preprocessing and exploration. Training and evaluating the model are the two main tasks
associated with data modelling, and are intended to achieve the goal of creating the
predictive/recognition system and to verify the accuracy and effectiveness of the model.
