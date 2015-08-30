# PhotoSlider for Swift

[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)

PhotoSlider can a simple photo slider and delete slider with swiping.


<img src="https://raw.githubusercontent.com/nakajijapan/PhotoSlider/master/demo.gif" width="300" />


## Installation

PhotoSlider is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "PhotoSlider"
```

## Usage



```swift

func collectionView(collectionView: UICollectionView, didSelectItemAtIndexPath indexPath: NSIndexPath) {

    var slider = PhotoSlider.ViewController(imageURLs: self.images)
    slider.modalPresentationStyle = .OverCurrentContext
    slider.modalTransitionStyle = UIModalTransitionStyle.CrossDissolve
    slider.index = indexPath.row
    self.presentViewController(slider, animated: true, completion: nil)

}

```

## Requirements
Xcode 6 is required.

## Author

nakajijapan, pp.kupepo.gattyanmo@gmail.com

## License

PhotoSlider is available under the MIT license. See the LICENSE file for more info.
