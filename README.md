![sharaku_header](https://github.com/makomori/Sharaku/blob/master/sharaku_header_big.png)

# Sharaku

[![CI Status](http://img.shields.io/travis/makomori/Sharaku.svg?style=flat)](https://travis-ci.org/makomori/Sharaku)
[![Version](https://img.shields.io/cocoapods/v/Sharaku.svg?style=flat)](http://cocoapods.org/pods/Sharaku)
[![License](https://img.shields.io/cocoapods/l/Sharaku.svg?style=flat)](http://cocoapods.org/pods/Sharaku)
[![Platform](https://img.shields.io/cocoapods/p/Sharaku.svg?style=flat)](http://cocoapods.org/pods/Sharaku)

## Usage
``` Swift
let imageToBeFiltered = UIImage(named: "targetImage")
let vc = SHViewController(image: imageToBeFiltered)
vc.delegate = self
self.present(vc, animated:true, completion: nil)
```

```
extension ViewController: SHViewControllerDelegate {
    func shViewControllerImageDidFilter(image: UIImage) {
      // Filtered image will be returned here.
    }

    func shViewControllerDidCancel() {
      // This will be called when your cancel filtering the image.
    }
}
```

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

Sharaku is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "Sharaku"
```

## Author

makomori, makomori26@gmail.com

## License

Sharaku is available under the MIT license. See the LICENSE file for more info.
