We have provided the both pyhton as well as ipynb files.
The python files are directly downloaded from colab, 
hence we recommend using jupyter notebooks for seeing the flow and running of the code.
The data is taken from chemical data and diseases data from cambridge's github and can be found here :
 https://github.com/cambridgeltl/MTL-Bioinformatics-2016/tree/master/data   
The files are to be run in the following order :

1) first run preprocess to get the weakly labelled data created using pubmed site data which was unlabelled : python preprocess.py
2) run MLM_training.ipynb -> pre-training step
3) run bert_crf_score.ipynb -> replacing with crf head and getting viterbi score
4) run NoiseRemovel.ipynb -> confidence interval based noise reduction
5) run selfTrain.ipynb -> self supervised training
6) run fineTuning.ipynb -> fine tuning

The models(only best models) and other intermediate results can be found in the following repository :
https://drive.google.com/drive/folders/1gnrK4E0okkUKO2M8_XKA4Xq04Q91ifpO?usp=drive_link
