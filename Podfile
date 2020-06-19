# Uncomment the next line to define a global platform for your project
platform :ios, '11.0'

target 'SampleProject' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  use_modular_headers!

  pod 'Firebase/Core'
  pod 'Firebase/Performance'
  pod 'Firebase/RemoteConfig'
  pod 'Firebase/Analytics'
  pod 'Firebase/Crashlytics'
  pod 'Firebase/Messaging'

  pod 'PromisesSwift'

  script_phase :name => 'Crashlytics',
              :script => '"${PODS_ROOT}/FirebaseCrashlytics/run"',
              :input_files => [
                '${DWARF_DSYM_FOLDER_PATH}/${DWARF_DSYM_FILE_NAME}/Contents/Resources/DWARF/${TARGET_NAME}',
                '$(SRCROOT)/$(BUILT_PRODUCTS_DIR)/$(INFOPLIST_PATH)'
              ]

end
