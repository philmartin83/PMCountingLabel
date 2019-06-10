# PMCountingLabel

This is a subclass of UILabel and when used can be used for counting as a timer or some sort of score display.
To use follow these steps

```swift
let counter = PMCountingLabel()
```

// add to the subview as normal then call count function

like so:
```swift
counter.count(fromValue: 1, to: castScoreToFloat, withDuration: 5, withAnimationType: .EaseOut, withCounterType: .Int)
```

fromValue: the number you wish the counter to start from
to: the number you wish the counter to stop at 
withDuration: the length of the time the counter should run for until it reaches its maximum value
animationType: the style of animation
counterType: if you require float values to display or int values to display

Animation Type:

there are currently 3 options of animation:
      Liner
      Ease In
      Ease Out
      
```swift      
//MARK:- Enums
    //MARK: Animation Type
    enum PMCounterAnimationType {
        // add the ability to change our animation
        case Linear
        case EaseIn
        case EaseOut
    }
    
    //MARK: Counter Type
    enum PMCounterType{
        case Int
        case Float
    }
```
