source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/artsy/Specs.git'

plugin 'cocoapods-keys', {
  :project => 'Eidolon',
  :keys => [
    'ArtsyAPIClientSecret',
    'ArtsyAPIClientKey',
    'HockeyProductionSecret',
    'HockeyBetaSecret',
    'MixpanelProductionAPIClientKey',
    'MixpanelStagingAPIClientKey',
    'CardflightAPIClientKey',
    'CardflightMerchantAccountToken',
    'StripePublishableKey'
  ]
}

platform :ios, '8.0'
use_frameworks!

# Yep.
inhibit_all_warnings!

# Artsy stuff
pod 'Artsy+UIColors'
pod 'Artsy+UILabels'
pod 'Artsy-UIButtons'

if ['orta', 'ash', 'artsy', 'Laura', 'CI', 'distiller'].include?(ENV['USER'])
    pod 'Artsy+UIFonts', '~> 1.1.0'
else
    pod 'Artsy+OSSUIFonts', '~> 1.1.0'
end

pod 'ORStackView'
pod 'FLKAutoLayout'
pod 'ISO8601DateFormatter', '0.7'
pod 'ARCollectionViewMasonryLayout', '~> 2.0.0'
pod 'SDWebImage', '~> 3.7'
pod 'SVProgressHUD', :git => 'https://github.com/ashfurrow/SVProgressHUD.git' # TODO: use official instead
pod 'RACAlertAction'

pod 'HockeySDK'
pod 'ARAnalytics/Mixpanel'
pod 'ARAnalytics/HockeyApp'

pod 'CardFlight'
pod 'Stripe'
pod 'ECPhoneNumberFormatter'
pod 'UIImageViewAligned', :git => 'https://github.com/ashfurrow/UIImageViewAligned.git'
pod 'DZNWebViewController', :git => 'https://github.com/orta/DZNWebViewController.git'
pod 'Reachability', :git => 'https://github.com/ashfurrow/Reachability.git', :branch => 'frameworks'

pod 'UIView+BooleanAnimations'
pod 'ARTiledImageView', :git => 'https://github.com/ashfurrow/ARTiledImageView.git'
pod 'XNGMarkdownParser'

# Swift indirect dependencies we need to force to Swift 2
pod 'Box', :head
pod 'Result', :head

# Swift pods
pod 'SwiftyJSON', :git => 'https://github.com/SwiftyJSON/SwiftyJSON.git', :branch => 'xcode7'
pod 'Alamofire', :git => 'https://github.com/Alamofire/Alamofire.git', :branch => 'swift-2.0'
pod 'ReactiveCocoa', :git => 'https://github.com/ashfurrow/ReactiveCocoa.git', :branch => 'swift2'
pod 'Moya/ReactiveCocoa', :git => 'https://github.com/Moya/Moya.git', :branch => 'swift-2.0'
pod 'Swift-RAC-Macros'
pod 'Dollar', :git => 'https://github.com/ashfurrow/Dollar.swift.git', :branch => 'swift-2-xcode-7'
pod 'Cent', :git => 'https://github.com/ashfurrow/Dollar.swift.git',:branch => 'swift-2-xcode-7'

target 'KioskTests' do

  pod 'FBSnapshotTestCase'
  pod 'Nimble-Snapshots'
  pod 'Quick'
  pod 'Nimble'
  pod 'Forgeries'

end
