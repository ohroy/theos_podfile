# Uncomment the next line to define a global platform for your project
platform :ios, '12.0'
install! 'cocoapods', :integrate_targets => false
post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
      config.build_settings['GCC_SYMBOLS_PRIVATE_EXTERN'] = 'NO'
    end
  end
end
target 'test' do
  # Comment the next line if you don't want to use dynamic frameworks
  #use_frameworks!
  pod 'Protobuf'
  # Pods for test
end
