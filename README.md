# Pytorch-Matching-Networks

Please look into the Jupyter Notebook to understand the Matching networks implementation for one-shot omniglot Classification

#TODO Items
<s>Make dataloader - To speed up training</s> - DONE - Loading all the numpy images at start speeds up things by a TON <br>
<s>Figure out what optimizer was used - SGD/ADAM? </s>- ADAM WORKS <br>
#<s>Use image augmentation </s> - Done <br>
<s>There is still something wrong with the network - Probably something with the way augmentation is done?</s> There isn't a problem with augmentation, rather the training and testing set provided by default have different "distributions". Need to investigate this further. Fixed by mixing the provided test and train set and creating new Train/Dev/Test sets. <br>
<s>Setup a way to log training of models</s> - Done via integraion with comet.ml <br>
Setup Hyperparameter Optimization <br>
Use a high level pytorch API to setup training loops and Checkpointing - PyTorch Ignite <br>
Using a dense layer at the end during embedding was causing the network to converge faser and better - Figure out why <br>
<s>Work on the LSTM based embedding</s> - Done Albeit incorrectly <br>
Implement Custom LSTM Cell which has hidden weights which can accept concatenated input <br>
