## vim

- <https://github.com/chriskempson/base16-vim/blob/master/colors/base16-default-light.vim> `c1c3e6c`
- <https://github.com/chriskempson/base16-vim/blob/master/colors/base16-default-dark.vim> `c1c3e6c`

```
3,10d | 4d | 5d | 36d | 42,49d |
4s#.*/#execute "silent !/bin/sh $HOME/.nightshell/# |
4s/\.sh// |
%s/base16-default/9009/ |

%s/181818/1f1e19/ |
%s/282828/302f28/ |
%s/383838/524f44/ |
%s/585858/706f67/ |
%s/b8b8b8/99978d/ |
%s/d8d8d8/bfbdb0/ |
%s/e8e8e8/e8e7df/ |
%s/f8f8f8/fffdf5/ |

%s/ab4642/d45959/ |
%s/dc9656/d47c24/ |
%s/f7ca88/bf8f00/ |
%s/a1b56c/63944a/ |
%s/86c1b9/3e9494/ |
%s/7cafc2/608fbf/ |
%s/ba8baf/8f72ab/ |
%s/a16946/bf6f7c/ |

%s/Character",    s:gui08, "", s:cterm08/Character",    s:gui05, "", s:cterm05/ |
%s/Cursor",        s:gui00, s:gui05, s:cterm00, s:cterm05/Cursor",        s:gui00, s:gui04, s:cterm00, s:cterm04/ |
%s/CursorLineNr",  s:gui04, s:gui01, s:cterm04, s:cterm01/CursorLineNr",  s:gui00, s:gui03, s:cterm00, s:cterm03/ |
%s/Identifier",   s:gui08, "", s:cterm08, "", "none/Identifier",   s:gui05, "", s:cterm05, "", "bold/ |
%s/LineNr",        s:gui03, s:gui01, s:cterm03/LineNr",        s:gui04, s:gui01, s:cterm04/ |
%s/MatchParen",    "", s:gui03, "", s:cterm03/MatchParen",    s:gui00, s:gui03, s:cterm00, s:cterm03/ |
%s/Search",        s:gui03, s:gui0A, s:cterm03, s:cterm0A,  "", "")/Search",        s:gui00, s:gui0A, s:cterm00, s:cterm0A,  "", "")/ |
%s/statusline",    s:gui04, s:gui02, s:cterm04, s:cterm02/statusline",    s:gui00, s:gui04, s:cterm00, s:cterm04/ |
%s/StatusLineNC",  s:gui03, s:gui01, s:cterm03, s:cterm01/StatusLineNC",  s:gui05, s:gui01, s:cterm05, s:cterm01/ |
%s/Visual",        "", s:gui02, "", s:cterm02/Visual",        s:gui06, s:gui02, s:cterm06, s:cterm02/ |
%s/VisualNOS",     s:gui08, "", s:cterm08, "", ""/VisualNOS",     "", s:gui01, "", s:cterm01, "none"/ |
%s/WildMenu",      s:gui08, s:gui0A, s:cterm08, ""/WildMenu",      s:gui00, s:gui06, s:cterm00, s:cterm06/ |

normal =gg
```

## nightshell

- <https://raw.githubusercontent.com/chriskempson/base16-shell/master/scripts/base16-default-light.sh> `376294b`
- <https://raw.githubusercontent.com/chriskempson/base16-shell/master/scripts/base16-default-dark.sh> `376294b`

```
2,4d |

%s#18/18/18#1f/1e/19# |
%s#28/28/28#30/2f/28# |
%s#38/38/38#52/4f/44# |
%s#58/58/58#70/6f/67# |
%s#b8/b8/b8#99/97/8d# |
%s#d8/d8/d8#bf/bd/b0# |
%s#e8/e8/e8#e8/e7/df# |
%s#f8/f8/f8#ff/fd/f5# |

%s#ab/46/42#d4/59/59# |
%s#dc/96/56#d4/7c/24# |
%s#f7/ca/88#bf/8f/00# |
%s#a1/b5/6c#63/94/4a# |
%s#86/c1/b9#3e/94/94# |
%s#7c/af/c2#60/8f/bf# |
%s#ba/8b/af#8f/72/ab# |
%s#a1/69/46#bf/6f/7c# |

%s/181818/1f1e19/ge |
%s/383838/524f44/g |
%s/d8d8d8/bfbdb0/g |
%s/f8f8f8/fffdf5/ge |

call append(123,["",
"echo -ne '\\e]12;#99978d\\a'"]) |

if @% =~ 'dark' | 125s/99978d/706f67/ | endif
```
