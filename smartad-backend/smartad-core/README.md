
check installed play version
---------------------------------
```
/usr/local/play-2.2.2/play help
```

check play version
------------------

```
$ cat project/plugins.sbt | grep play
addSbtPlugin("com.typesafe.play" % "sbt-plugin" % "2.2.2")
```

run
-------

```
$ /usr/local/play-2.2.2/play compile
$ /usr/local/play-2.2.2/play "~run 8443"
```

api
--------

```
curl http://localhost:9000/products
```

using notification engine
---------------------------

```
var ws = new WebSocket("ws://localhost:9000/notification");
ws.onmessage = function( message ) { console.log( message ); };
ws.send("Prayag Upd is in Mountain View.");
```

Nerd Tools
-----------

[play.vim](https://github.com/rdolgushin/play.vim)

 |

 |____ [snipmate.vim](https://github.com/msanders/snipmate.vim)


[.vimrc](https://github.com/iPrayag/.dotfiles/blob/master/.vimrc)


They say copy `$PLAY_HOME/support/vim/*.snippets` to `~/.vim/bundle/vundle/snippets/`  , [official documentation](http://www.playframework.com/documentation/1.2.3/ide)


Motivation
--------------
[Vim Plugins You Should Know About, Part IV: snipmate.vim, Peteris Krumins](http://www.catonmat.net/blog/vim-plugins-snipmate-vim/)
