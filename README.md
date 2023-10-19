# Setup multiple PHP Versions on macOS
Setup multiple PHP Versions on macOS

✅ Method One :
There are a few open source projects that aim to automate this for you :

[phpbrew/phpbrew](https://dlgram.com/OTyzq)

[philcook/brew-php-switcher](https://dlgram.com/CPqmf)




--------------------------------------------------------------------------------------------


✅ Method Two :

- install the XCode Command Line Tools :
```
   xcode-select --install
```  

 - install Brew :

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```  

- Please check with the following command if brew has been successfully installed:
```
brew --version
```

- Next, you can install all the PHP versions you need.
```
brew install shivammathur/php/php@5.6
brew install shivammathur/php/php@7.0
brew install shivammathur/php/php@7.1
brew install shivammathur/php/php@7.2
brew install shivammathur/php/php@7.3
brew install shivammathur/php/php@7.4
brew install shivammathur/php/php@8.0
```

- To switch between the PHP versions ( example switch from PHP 7.4 to PHP 5.6 ):
 ```
brew unlink php@7.4 && brew link --force —-overwrite php@5.6

```

