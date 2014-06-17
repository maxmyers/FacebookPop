#5 Steps For Using Facebook Pop#
  ```objective-c
    // 1. Pick a Kind Of Animation //  POPBasicAnimation  POPSpringAnimation POPDecayAnimation
    
    POPSpringAnimation *basicAniamtion = [POPSpringAnimation animation];
    
    
    // 2. Decide weather you will animate a view property or layer property, Lets pick a View Property and pick kPOPViewFrame
    
    // View Properties - kPOPViewAlpha kPOPViewBackgroundColor kPOPViewBounds kPOPViewCenter kPOPViewFrame kPOPViewScaleXY kPOPViewSize
    
    // Layer Properties - kPOPLayerBackgroundColor kPOPLayerBounds kPOPLayerScaleXY kPOPLayerSize kPOPLayerOpacity kPOPLayerPosition kPOPLayerPositionX kPOPLayerPositionY kPOPLayerRotation kPOPLayerBackgroundColor
    
    basicAniamtion.property = [POPAnimatableProperty propertyWithName:kPOPViewFrame];
    
    
    
    // 3. Figure Out which of 3 ways to set toValue
    
    //  anim.toValue = @(1.0);
    //  anim.toValue =  [NSValue valueWithCGRect:CGRectMake(0, 0, 400, 400)];
    //  anim.toValue =  [NSValue valueWithCGSize:CGSizeMake(40, 40)];
    
    basicAniamtion.toValue=[NSValue valueWithCGRect:CGRectMake(0, 0, 90, 190)];
    
    
    
    // 4. Create Name For Animation
    
    basicAniamtion.name=@"hiiidd";
    
    
    // 5. Add animation to View or Layer, we picked View so self.tableView and not layer which would have been self.tableView.layer
    
    [self.tableView pop_addAnimation:basicAniamtion forKey:@"WhatEverNameYouWant"];
  ```


## Step 1 Pick Kind of Animation


### POPBasicAnimation
 ```objective-c
 POPBasicAnimation *basicAniamtion = [POPBasicAnimation animation];
 basicAniamtion.duration=3;
 ```
 
### POPSpringAnimation
  ```objective-c
  POPSpringAnimation *springAnimation = [POPSpringAnimation animation];
 springAnimation.velocity=@(1000);       // change of value units per second
 springAnimation.springBounciness=14;    // value between 0-20 default at 4
 springAnimation.springSpeed=3;     // value between 0-20 default at 4
  ```
### POPDecayAnimation
```objective-c
 POPDecayAnimation *decayAnimation=[POPDecayAnimation animation];
 decayAnimation.velocity=@(233); //change of value units per second
 decayAnimation.deceleration=.833; //range of 0 to 1
  ```
### Example
```objective-c
 POPBasicAnimation *basicAniamtion = [POPBasicAnimation animation];
  ```

## Step 2 Decide weather you will animate a view property or layer property

### View Properties


##### Alpha - kPOPViewAlpha
##### Color - kPOPViewBackgroundColor
##### Size - kPOPViewBounds
##### Center - kPOPViewCenter 
##### Location & Size - kPOPViewFrame
##### Size - kPOPViewScaleXY
##### Size(Scale) - kPOPViewSize


### Layer Properties
##### kPOPLayerBackgroundColor 
##### kPOPLayerBounds 
##### kPOPLayerScaleXY 
##### kPOPLayerSize 
##### kPOPLayerOpacity 
##### kPOPLayerPosition 
##### kPOPLayerPositionX 
##### kPOPLayerPositionY 
##### kPOPLayerRotation 
##### kPOPLayerBackgroundColor
