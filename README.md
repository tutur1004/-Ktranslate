# $Ktranslate
$Ktranslate, an skript addons in skript !

Make your server international !!

With $Ktranslate you can set differents messages for differents langages players.

## How to use $Ktranslate

### Command:
```yml
/lang [<lang name>]
Desc: set your lang
Perms: no permissions, all players can use it !

/lang reload
Desc: reload config, ne need to reload when you change a traduction, only when you add new lang or changing default language
Perms: sktranslate.lang-reload
```

### Use in Skript:
$Ktranslate can use in all send effects `(send|message)`.
Just need to paste `%translate(player, "here-put-your-index-name")%`
```yml
#Exemple
send "%translate(player, "exemple-message1")%" to player
```
The Skript just upside send `exemple-message1` in the lang of player!

### Set traduction in translate.yml
If you want add a message to say `mutation is done`, exemple for a skript named `hero`
in file translate.yml you just need to insert:
```yml
français:
    #Insert this part:
    hero-mutation-done: "Mutation effectuée"

english:
    #Insert this part:
    hero-mutation-done: "Mutation is done"
```

### Add new languages in translate.yml
Probably the most simple part of this addon.
But be sure that this is the longest part to do x)
```yml
#Start by adding lang in lang list:
lang-list:
- français
- english
- yournewlang

#and after add the lang:

français:
    #Some traductions

english:
    #Some traductions

yournewlang:
    #Some traductions
```
After reload config, be sure all traduction where set in `yournewlang`!!! it's very important !!!
