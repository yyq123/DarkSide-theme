# DarkSide for [ConEmu](http://conemu.github.io)

> A dark theme for [ConEmu](http://conemu.github.io) based on [DraculaTheme](https://draculatheme.com/conemu) .

![Screenshot](https://yyq123.github.io/DarkSide-theme/conemu/DarkSide-ConEmu.png)

## Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

`$ git clone https://github.com/yyq123/DarkSide-theme.git`

## Install manually

Download using the GitHub .zip download option and unzip them.

## Activating theme 激活主题

You have to manually modify the ConEmu config file. 需要手工修改ConEmu配置文件。

1. Open ConEmu.xml file. It is in the installation directory of ConEmu or the user directory like C:\Users\UserName. 打开ConEmu.xml文件，此文件通常存放在 ConEmu安装目录或用户主目录中。
![Screenshot](https://yyq123.github.io/DarkSide-theme/conemu/DarkSide-ConEmu-Settings-Colors.png)
2. Find the palette definition. It is a xml tag starts with the following code: 查找类似以下的色彩定义代码：

```
<value name="ColorTable00" type="dword" data="00131313"/>
<value name="ColorTable01" type="dword" data="00bc4354"/>
<value name="ColorTable02" type="dword" data="00808080"/>
<value name="ColorTable03" type="dword" data="00fbd677"/>
<value name="ColorTable04" type="dword" data="00967adc"/>
<value name="ColorTable05" type="dword" data="00f993bd"/>
<value name="ColorTable06" type="dword" data="006cb8ff"/>
<value name="ColorTable07" type="dword" data="00f2f8f8"/>
<value name="ColorTable08" type="dword" data="009e6753"/>
<value name="ColorTable09" type="dword" data="00cd0000"/>
<value name="ColorTable10" type="dword" data="00c89d57"/>
<value name="ColorTable11" type="dword" data="00ed9564"/>
<value name="ColorTable12" type="dword" data="005555ff"/>
<value name="ColorTable13" type="dword" data="00c679ff"/>
<value name="ColorTable14" type="dword" data="008cfaf1"/>
<value name="ColorTable15" type="dword" data="00f2f8f8"/>
<value name="ColorTable16" type="dword" data="00000000"/>
<value name="ColorTable17" type="dword" data="00800000"/>
<value name="ColorTable18" type="dword" data="00008000"/>
<value name="ColorTable19" type="dword" data="00808000"/>
<value name="ColorTable20" type="dword" data="00000080"/>
<value name="ColorTable21" type="dword" data="00800080"/>
<value name="ColorTable22" type="dword" data="00008080"/>
<value name="ColorTable23" type="dword" data="00c0c0c0"/>
<value name="ColorTable24" type="dword" data="00808080"/>
<value name="ColorTable25" type="dword" data="00ff0000"/>
<value name="ColorTable26" type="dword" data="0000ff00"/>
<value name="ColorTable27" type="dword" data="00ffff00"/>
<value name="ColorTable28" type="dword" data="000000ff"/>
<value name="ColorTable29" type="dword" data="00ff00ff"/>
<value name="ColorTable30" type="dword" data="0000ffff"/>
<value name="ColorTable31" type="dword" data="00ffffff"/>
```

3. If you don't find the xml above, you may not have any custom color scheme. So open ConEmu Settings dialog (Win+Alt+P), and go to Features -> Colors -> Schemes, enter a name and click Save, then the palette definition will be generated. Close ConEmu. 如果没有发现以上xml文件，那么你可以在ConEmu的Settings对话框中，选择Features -> Colors -> Schemes，然后输入名称DarkSide并点击Save按钮，以生成配置信息。
4. Replace the color table in the palette tag with the DarkSide color table (see conemu/DarkSide.xml, there are 32 color values), save the ConEmu.xml. 将文件中DarkSide色彩定义部分，替换为以上代码（或参考 conemu/DarkSide.xml 文件, 共计32个色彩定义），保存文件。
5. Reopen ConEmu. 重新启动Conemu。
6. Notice that ConEmu's color scheme may not change in the later version, because the <Current color scheme> is used by ConEmu instead of the DarkSide, you need to go to Features -> Colors -> Schemes and switch to DarkSide. 如果色彩仍无变化，请确认Features -> Colors -> Schemes是否已选中DarkSide。
