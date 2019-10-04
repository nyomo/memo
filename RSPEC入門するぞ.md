https://bundler.io/v2.0/guides/creating_gem.html

Gemfileにはspecfileだけ書かれていれば良さそう
Gemfile.lockに書かれていることがGemfileより優先されるっぽい

クラスメソッドでは無くインスタンスメソッドにして居るのはインスタンス変数を使っているのでインスタンスの状態以外で呼ばれたく無いという説明をつねさまにした

bundle exec rspec spec

spec/slack_goodies_spec.rb を作った

https://qiita.com/jnchito/items/640f17e124ab263a54dd

↑の通りにやると良さそうだけど、initializeでいきなりAPIを呼ばないでnewしてからAPI呼び出すようにした方が良さそう