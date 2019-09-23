# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: 在我们开始之前, 你的阅读习惯是...?

`publish("show_options_bottom")`

# intro-start-2

n3: 现在，让我们开始吧...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: 这是一个人类。

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: 这是他的焦虑

n: 你，就是他的焦虑

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nope. No, nope, not listening. Gonna check my phone.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: 你的职责就是保护他不受伤害！

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Gasp! You're scrolling your life away on Twitter! Again!嘿！你的生命就在推特上被这么一点一点的划走了！又一次！

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Yeah I wonder why I don't just sit and listen to my thoughts more often.是啊，我就想知道为啥我不坐下来多听听我脑子里的想法。

`hong({eyes:"neutral"});`

n: QUICK, WARN THEM ABOUT A *DANGER!* 快！快告诉她危险！

```
bb({eyes:"look"});
```

[天哪，这个故事太可怕了！](#act1d_news)

[ 嗯？那条推特实在偷偷讨论我吗？](#act1d_subtweet)

[嘿，一个喵星人喝牛奶的GIF！](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: 噢好可爱啊，我...

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: 猫是不能消化牛奶的！我们是虐待动物的人！！

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



