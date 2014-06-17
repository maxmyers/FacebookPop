<h1>5 Steps For Using Facebook Pop</h1>

## Step 1 Pick Kind of Animation

#### POPBasicAnimation
 ```objective-c
 POPBasicAnimation *basicAniamtion = [POPBasicAnimation animation];
 basicAniamtion.duration=3;
 ```
 
#### POPSpringAnimation
  ```objective-c
  POPSpringAnimation *springAnimation = [POPSpringAnimation animation];
 springAnimation.velocity=@(1000);       // change of value units per second
 springAnimation.springBounciness=14;    // value between 0-20 default at 4
 springAnimation.springSpeed=3;     // value between 0-20 default at 4
  ```
#### POPDecayAnimation
```objective-c
 POPDecayAnimation *decayAnimation=[POPDecayAnimation animation];
 decayAnimation.velocity=@(233); //change of value units per second
 decayAnimation.deceleration=.833; //range of 0 to 1
  ```

## Step 2 Decide weather you will animate a view property or layer property

#### View Properties
```objective-c
kPOPViewAlpha 
kPOPViewBackgroundColor 
kPOPViewBounds 
kPOPViewCenter 
kPOPViewFrame 
kPOPViewScaleXY 
kPOPViewSize
```
#### Layer Properties
##### ∙kPOPLayerBackgroundColor 
##### ∙kPOPLayerBounds 
##### ∙kPOPLayerScaleXY 
##### ∙kPOPLayerSize 
##### ∙kPOPLayerOpacity 
##### ∙kPOPLayerPosition 
##### ∙kPOPLayerPositionX 
##### ∙kPOPLayerPositionY 
##### ∙kPOPLayerRotation 
##### ∙kPOPLayerBackgroundColor
