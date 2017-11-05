source "https://github.com/CocoaPods/Specs"
platform :ios, '9.0'

target 'TestProject' do
  use_frameworks!
  
  pod 'AlamofireObjectMapper', '~> 4.0'
  pod 'XCGLogger', '~>5.0.1'
  pod 'SwiftyJSON'
  pod 'Alamofire'

  target 'TestProjectTests' do
    inherit! :search_paths
  end

  target 'TestProjectUITests' do
    inherit! :search_paths
  end

end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end
