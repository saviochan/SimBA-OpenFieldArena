# SimBA-OpenFieldArena
Rearing classifier for mouse in open field arena with 8 body parts labelled 

<p align="center">
  <img src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/gifs/Rearing.gif">
</p>

### Model Settings

The labelling schematics for this model is 8 body parts on a single mouse recorded 90° above angle. To optimize performance, a threshold probability p=0.313 and a minimum bout duration(rearing)=300ms should be used.

<img align="left" width="300"  src="https://github.com/saviochan/Deeplabcut-OpenFieldArena/blob/master/images/Labelling.png"><img align="left" width="300"  src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Model%20settings.jpg"><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>


### Model evaluation

The model was built with 19058 manually annotated rearing frames(~13% of total frames). 
Using a train test split method(all video frames are grouped together and randomly split such that 80% of frames for training and 20% of frames for testing), the trained model has a F1 score=0.71, a precision=0.68 and a recall=0.74.
Using a time series split( in each video, the first 80% of the frames are used for training and the last 20% of the frames are used for testing), the trained model has a F1 score=0.67, a precision=0.66, a recall=0.67.

<img align="left" width="300" src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Curve.jpg">
<img align="left" width="300" src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Curve_2.jpg"><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

To further validate the performance of our model, we took a 25-min open field video(15000 frames) and scores the human-labelled result with the machine-labelled result.

<img align="left" width="1000" src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/Comparison.jpg">
<img align="left" width="1000" src="https://github.com/saviochan/SimBA-OpenFieldArena/blob/master/images/chart.jpg">

More evaluation files can be found [here.](/models/generated_models/model_evaluations)

### Downloads
The rearing model can be downloaded on Zenodo: https://zenodo.org/record/3964701#.XyB8OJ5KhPY
