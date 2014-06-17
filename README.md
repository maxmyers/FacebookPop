<h1>FacebookPop</h1>


## 5 Steps For Using Facebook Pop



## 1 Pick Kind of Animation

 ## Request 
 ```objective-c
 POPBasicAnimation *basicAniamtion = [POPBasicAnimation animation];
 basicAniamtion.duration=3;
 ```
 
 POPSpringAnimation 
  ```objective-c
  POPSpringAnimation *springAnimation = [POPSpringAnimation animation];
 springAnimation.velocity=@(1000);       // change of value units per second
 springAnimation.springBounciness=14;    // value between 0-20 default at 4
 springAnimation.springSpeed=3;     // value between 0-20 default at 4
  ```
 POPDecayAnimation


```objective-c
 POPBasicAnimation *basicAniamtion = [POPBasicAnimation animation];
 basicAniamtion.duration=3;
 


 
 POPSpringAnimation *springAnimation = [POPSpringAnimation animation];
 springAnimation.velocity=@(1000);       // change of value units per second
 springAnimation.springBounciness=14;    // value between 0-20 default at 4
 springAnimation.springSpeed=3;     // value between 0-20 default at 4
 



 
 POPDecayAnimation *decayAnimation=[POPDecayAnimation animation];
 decayAnimation.velocity=@(233); //change of value units per second
 decayAnimation.deceleration=.833; //range of 0 to 1
```

