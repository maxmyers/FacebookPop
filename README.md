<h1>FacebookPop</h1>


## 5 Steps For Using Facebook Pop



## 1 Pick Kind of Animation

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

#### Request
```objective-c
 POPDecayAnimation *decayAnimation=[POPDecayAnimation animation];
 decayAnimation.velocity=@(233); //change of value units per second
 decayAnimation.deceleration=.833; //range of 0 to 1
  ```



```

`AFHTTPRequestOperationManager` encapsulates the common patterns of communicating with a web application over HTTP, including request creation, response serialization, network reachability monitoring, and security, as well as request operation management.

#### `GET` Request

```objective-c
AFHTTPRequestOperationManager *manager = [AFHTTPRequestOperationManager manager];
[manager GET:@"http://example.com/resources.json" parameters:nil success:^(AFHTTPRequestOperation *operation, id responseObject) {
    NSLog(@"JSON: %@", responseObject);
} failure:^(AFHTTPRequestOperation *operation, NSError *error) {
    NSLog(@"Error: %@", error);
}];
```
