# Uncomment this line to define a global platform for your project

use_frameworks! :linkage => :static

abstract_target 'MatrixSDK' do
    
    pod 'AFNetworking', '~> 4.0.0'
    pod 'GZIP', '~> 1.2.2'

    pod 'OLMKit', :git => 'https://collaborate.uhnresearch.ca/stash/scm/coco/olm.git', :commit => '78b56ffe29bcf0e56e3b85fbf695b841b545e48a', :inhibit_warnings => true
    #pod 'OLMKit', '~> 3.1.0', :inhibit_warnings => true
    #pod 'OLMKit', :path => '../olm/OLMKit.podspec'
    
    pod 'Realm', '~> 4.4.0'
    pod 'libbase58', '~> 0.1.4'
    
    target 'MatrixSDK-iOS' do
        platform :ios, '9.0'
        
        target 'MatrixSDKTests-iOS' do
            inherit! :search_paths
            pod 'OHHTTPStubs', '~> 9.0.0'
        end
    end
    
    target 'MatrixSDK-macOS' do
        platform :osx, '10.10'

        target 'MatrixSDKTests-macOS' do
            inherit! :search_paths
            pod 'OHHTTPStubs', '~> 9.0.0'
        end
    end
end
