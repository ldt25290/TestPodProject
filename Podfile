platform :ios, '11.0'

use_frameworks!

workspace 'TestPodProject'

#core module
def core_pods
    pod 'RxSwift'
end

target 'Core' do
    project 'Common/Core/Core.project'
    core_pods
end

#login feature module
def login_feature_pods
    core_pods
end

target 'LoginFeature' do
    project 'Modules/LoginFeature/LoginFeature.project'
    login_feature_pods
end

#user profile feature module
def user_profile_feature_pods
    core_pods
end

target 'UserProfileFeature' do
    project 'Modules/UserProfileFeature/UserProfileFeature.project'
    user_profile_feature_pods
end

#application
def application_pods
  login_feature_pods
  user_profile_feature_pods
  core_pods
end

target 'TestPodProject' do
  project 'App/TestPodProject/TestPodProject.project' 
  application_pods
  # Pods for Application

end
