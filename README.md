# PhotoSlider for Swift 2

[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)

PhotoSlider can a simple photo slider and delete slider with swiping.



<img src="https://raw.githubusercontent.com/nakajijapan/PhotoSlider/master/demo.gif" width="300" />



## Installation

PhotoSlider is available through [Carthage](https://github.com/Carthage/Carthage). 

To install it, simply add the following line to your Cartfile:

``` ruby
github "metodowhite/PhotoSlider" "0.5.1"
```

## Usage



``` swift

func collectionView(collectionView: UICollectionView, didSelectItemAtIndexPath indexPath: NSIndexPath) {

    var slider = PhotoSlider.ViewController(imageURLs: self.images)
    slider.modalPresentationStyle = .OverCurrentContext
    slider.modalTransitionStyle = UIModalTransitionStyle.CrossDissolve
    slider.index = indexPath.row
    self.presentViewController(slider, animated: true, completion: nil)

}

```

## Requirements

Xcode 7 & Swift 2 is required.

## Original Author

nakajijapan, pp.kupepo.gattyanmo@gmail.com

heavily modified to use [Carthage](https://github.com/Carthage/Carthage), [Kingfisher](https://github.com/onevcat/Kingfisher) instead [SDWebImage](https://github.com/rs/SDWebImage), and Swift 2.

## License

PhotoSlider is available under the MIT license. See the LICENSE file for more info.