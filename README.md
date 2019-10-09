# git_color

## bashrc
### export CLICOLOR=1  
  显示颜色

### export PS1='\[\033[1;31m\]\u@\h: \[\033[0;33m\]\A \[\033[36m\]\w # \[\033[0;38m\]'  
  显示当前用户和目录，并匹配颜色

### enable color support of ls and also add handy aliases
if [ -x /usr/bin/dircolors ]; then
    test -r ~/.dircolors && eval "$(dircolors -b ~/.dircolors)" || eval "$(dircolors -b)"
    alias ls='ls --color=auto'
    #alias dir='dir --color=auto'
    #alias vdir='vdir --color=auto'

    alias grep='grep --color=auto'
    alias fgrep='fgrep --color=auto'
    alias egrep='egrep --color=auto'
fi

## dircolors文件就是上面提到的./dircolors

## reference list 
### https://github.com/seebi/dircolors-solarized/blob/master/README.md  
a awesome project 
### https://www.jianshu.com/p/0f556c6c4ec8  
a very clear tutorial  
