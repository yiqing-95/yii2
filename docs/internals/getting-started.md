Getting started with Yii2 development
=====================================

The best way to have a locally runnable webapp that uses codebase cloned from main repository is to use `yii2-dev`
Composer package. Here's how to do it:

1. `git clone git@github.com:yiisoft/yii2-app-basic.git`.
2. Remove `.git` directory from cloned directory.
3. Change `composer.json`. Instead of all stable requirements add just one `"yiisoft/yii2-dev": "*"`.
4. Execute `composer install`.
5. Now you have working playground that uses latest code.

If you're core developer there's no extra step needed. You can change framework code under
`vendor/yiisoft/yii2-dev` and push it to main repository.

If you're not core developer or want to use your own fork for pull requests:

1. Fork `https://github.com/yiisoft/yii2` and get your own repository address such as
   `git://github.com/username/yii2.git`.
2. Edit `vendor/yiisoft/yii2-dev/.git/config`. Change remote `origin` url to your own:

```
[remote "origin"]
  url = git://github.com/username/yii2.git
```
