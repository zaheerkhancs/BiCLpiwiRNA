# BiCLpiwiRNA
BiCLpiwiRNA: BiCascade Layered piwiRNA Predictor...
# A Brief
BiCLpiwiRNA model make use of different notion of k-mer as feature extraction technique and Multi Layered perceptron  as the dominant classification algorithm.  we have used two varient notion of feature selection via Sequential forward featuer selection of MLEXTEND and also Relief feature importance. The proposed model analysis result were simulated via both selected feature to bubble the top optimum features. Based on those optium feature a bi-layred model been developed.
The 1st layer discriminates a given piwiRNA sequence, if the query sequence is predicted as Enhancer then the 2nd Layer tries to predicts their TAREGET FUNCTION
## Getting Started

Following are list of todo, before making run of the propose model.

### Prerequisites
#####  Following are the lib need to be installed....
What things you need to install the software and how to install them
- python3.6  [follow](https://www.python.org/downloads/release/python-367/)
- keras 2.2.4 [follow](https://keras.io/)
- Flask 1.0.2 [follow](http://flask.pocoo.org/docs/0.12/installation/)
- scikit-learn 0.19.1 [follow](https://scikit-learn.org/stable/install.html)
- scipy 1.1.0 [follow](https://scipy.org/install.html)
- numpy1.15.4 [follow](https://docs.scipy.org/doc/numpy/user/install.html)
- matplotlib3.0.2 [follow](https://matplotlib.org/users/installing.html#building-on-windows/)
- tensorflow 1.12.0 [follow](https://www.tensorflow.org/hub/installation)

```
$pip install <lib_name>
```
### Get Various Features.

```
_GetVariousFeatures.py
```
_GetVariousFeatures.py is used for Get various features used in the proposed approach.

### Get Feature Selection

```
_GetSFSReliefFeatures.py
```
_GetSFSReliefFeatures.py is used for Get the selected featres via, SFS and relief feature selection importances method.


### Evaluate a model.

```
EvaluateModel.py
```
EvaluateModel.py is used for Evaluating a pre-trained model, stored for each successive layeres 1&2.


### Making prediction.

```
ModelPrediction.py
```
ModelPrediction.py is used to use to Obtained class probibilities for successive Layeres 1&2 on feeding and unseen Fasta Sequence or Sequence File.



# Also Cite
Z. U. Khan, D. Pi et al, “iRSpot-SPI: Deep learning-based recombination spots prediction by incorporating secondary sequence information coupled with physio-chemical properties via Chou’s 5-step rule and pseudo components,” Chemom. Intell. Lab. Syst., 2019.

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Inspiration
* etc.. Thanks to Professor.Pi for his Constructive Commments throughout all stages of this Paper.
