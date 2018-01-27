study-serverspec
================


準備
----

オンライン環境でgemをインストールする。

```sh
$ bundle init
$ cat <<'EOS' >> Gemfile
gem 'serverspec'
EOS
$ bundle install --path=vendor/bundle
```

インストールされたgemをローカル用に保存する。

```sh
$ bundle package
```

cacheに保存されたgemからgemをインストールする。

```sh
$ bundle install --path=vendor/bundle --local
```
