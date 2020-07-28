# SimBA-OpenFieldArena
Rearing classifier for mouse in open field arena with 8 body parts labelled 

<p align="center">
  <img src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/gifs/Rearing.gif">
</p>

## Model Settings

The labelling schematics for this model is 8 body parts on a single mouse recorded 90° above angle. To optimize performance, a threshold probability p=0.313 and a minimum bout duration(rearing)=300ms should be used.<br/>

<img align="left" width="480"  src="https://github.com/saviochan/Deeplabcut-OpenFieldArena/blob/master/images/Labelling.png">
<img align="left" width="480"  src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Model%20settings.jpg"><br/>

## Model evaluation

The model was built with 19058 manually annotated rearing frames(~13% of total frames). With a train-test ratio of 0.8, the trained model has a F1 score=0.71, a precision=0.68 and a recall=0.74.<br/>

<img align="left" width="450" src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Curve.jpg">
<img align="left" width="450" src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Curve_2.jpg"><br/>

To further validate the performance of our model, we took a 25-min open field video(15000 frames) and scores the human-labelled result with the machine-labelled result.

## Downloads
The rearing model can be downloaded on Zenodo: 
