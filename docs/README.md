# composer-version-constraint
Latest composer throwing version constraint error 

*Could not parse version constraint 5.5.33 as ^5.2: Invalid version string "^5.2"*

## Clone the repo to root folder where Magento2 root composer.json is installed
```shell script
git clone git@github.com:rapiddive/composer-version-constraint.git
```

## In root composer.json for Magento2
```composer log
{
    ...
    "autoload": {
        "files": [
            ...
            "composer-version-constraint/ComposerRepository.php"
            ...
        ],
    }
    ...
}
```
## Dump autoload
```shell script
composer dumpautoload
```

## Install any package causing issue with following command
```shell script
./vendor/bin/composer require vendor/packagename
```
