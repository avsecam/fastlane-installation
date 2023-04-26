# fastlane
## Windows without WSL
### Installing Ruby and fastlane
1. Install a version of [RubyInstaller](https://rubyinstaller.org/downloads/archives/) that is 2.5 or later. (fastlane supports only Ruby versions 2.5 or later)
2. Only the base files are required. ![](./images/ri-installer.png)
3. Check if Ruby is in your environment variables. ![](images/env.png)
4. In a terminal, run the following command to install fastlane and its dependencies. Note that this will add fastlane to the currently used Ruby version only. Use [RIDK](#ridk) to change versions.
   ```
 	gem install fastlane
5. You now have fastlane installed. 😄
   - In your project directory, you can now run fastlane commands. For example:
   ```
	fastlane android prepare

## Windows with WSL
### Enabling WSL
1. Search for "windows features" in your Start Menu and go to the following option. ![](images/windows-features-search.png)
2. Enable the "Windows Subsystem for Linux" option. ![](images/windows-features.png)
### Setting up Ruby and fastlane in a WSL terminal (You can also follow [these](https://docs.fastlane.tools/getting-started/android/setup/) steps instead)
1. Install a Ruby environment manager like [rbenv](https://github.com/rbenv/rbenv) or [RVM](https://rvm.io/) and install a Ruby version that is 2.5 or later. (fastlane supports only Ruby versions 2.5 or later)
2. Install Bundler.
   ```
	 gem install bundler
3. Install fastlane.
   ```
	 gem install fastlane

## Notes
### RIDK