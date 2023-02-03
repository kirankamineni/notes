# Installing ruby on an M2 Mac with Venture

Any system that uses `ruby-build` will run into issues if you are installing an older EOLed version of ruby (ex: 2.6.10)

So, 

1. Download 13.4.1 version of xcode from developer.apple.com
2. Unarchive the downloaded `.xip` file
3. `sudo xcode-select PATH-TO-THE-EXTRACTED.app`
4. Run the following command to install ruby
```sh
optflags=-Wno-error=implicit-function-declaration ASDF_RUBY_BUILD_VERSION=v20220630 asdf install ruby 2.6.10
```

