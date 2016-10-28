# Uncomment this line to define a global platform for your project
platform :ios, '10.0'
use_frameworks!

target 'mffw-mobile-app-v2' do
    pod 'ArcGIS-Runtime-SDK-iOS'
    pod 'SwiftHTTP', '2.0.1'
    pod 'SwiftyJSON', '3.0.0'
    pod 'SLExpandableTableView'
    pod 'Charts', '~> 3.0'
    pod 'MBProgressHUD'
    pod 'Fabric'
    pod 'Crashlytics'
    pod 'Appsee'
    pod 'SwiftValidator', :git => 'https://github.com/jpotts18/SwiftValidator.git', :branch => 'master'
    pod 'SWRevealViewController', '~> 2.3'
    pod 'R.swift' , '~> 3.1'
end

target 'mffw-mobile-app-v2Tests' do

end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end
