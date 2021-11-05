## 自己用的zsh设置：
1. 安装zsh，mac 自带，linux一般用ubuntu，用下面的命令:
> apt install zsh

2. 安装oh-my-zsh:
> sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

或者：

> sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"

3. 安装高亮的插件zsh-syntax-highlighting：
> git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/plugins/zsh-syntax-highlighting

4. 修改~/.zshrc文件,下面几个是自己常用的：
plugins=(zsh-syntax-highlighting z git sudo)

5. 增加自动补全的功能：（incr-0.2是原版，incr是修改版）

> mkdir ~/.oh-my-zsh/plugins/incr

> wget https://raw.githubusercontent.com/gudk/zsh_config/master/incr/incr.zsh -O ~/.oh-my-zsh/plugins/incr/incr.zsh

6. 修改.zshrc，启用自动补全：
> echo "source ~/.oh-my-zsh/plugins/incr/incr*.zsh" >> ~/.zshrc

7.安装powerlevel10k:

> git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

8. 修改主题为p10k：

> ZSH_THEME="powerlevel10k/powerlevel10k"

9. 复制.p10k.zsh

> wget https://raw.githubusercontent.com/gudk/zsh_config/master/.p10k.zsh -O ~/

10. source ~/.zshrc 更新配置。

11.暂时就这些。
