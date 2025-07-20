### AWS Models 

These models are in a bucket s3 bucket called s3://shared-public-model-artifacts-crljaso/aneurysm_rupture_classification/. You can use them by s3 copying them in the aws cli into a jupyter notebook running on sagemaker and then using TabularPredictor.load(path) on a folder path like to autogluon_models_round_two1. This will make it by default use the best model trained when called model.predict() but it can be changed to use any other model autogluon trained. Note that you will need to install the same autogluon version used to train the model. You will get an error with this version if you don't have it... simply restart the kerned and use %pip install autogluon==1.x.y at the top cell where x and y are the intended versions.

