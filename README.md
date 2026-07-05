# rime-dict-Otter
面向rime的游戏词库，目前包含DotA2、原神（Genshin Impact）、绝区零（Zenless Zone Zero）。
*来是只有DotA2的，后来索性把玩的游戏都给放上来好了。*

## 背景

个人喜爱DotA2这款游戏，但是网络上似乎没有一款及时更新的简体中文DotA2词库。所以就充分利用个人空闲时间，制作了这份DotA2词库，供RIME输入法的朋友们使用。
另外，此词库目前会同步更新到搜狗拼音输入法的词库「[DotA2词库、刀塔2](https://pinyin.sogou.com/dict/detail/index/109151)」中。
原神和绝区零实在是懒得更新上去了，有需求的可以通过深蓝词库转换工具自行转换为搜狗的格式。

## 使用方法
### 词库的使用
#### 首次使用词库：
1. 下载本项目`custom-dicts`文件夹下制作的词库文件，例如`RIMEDotA2.dict.yaml`；
2. 将下载的文件放置到「用户文件夹」下的`custom-dicts`文件夹中（例如`%appdata%\Rime\custom-dicts\RIMEDotA2.dict.yaml`）；
3. 打开输入方案词库设置文件（例如`%appdata%\Rime\rime_ice.dict.yaml`）；
4. 在`import_tables:`下添加本词库`  - custom-dicts/RIMEDotA2`。

![引入词库示例图片](https://github.com/user-attachments/assets/876844bc-1541-4bcf-9dec-f276632ac2eb)

> 上图中，将词库文件放置在了单独的文件夹`custom-dicts`中；实际使用时，也可以不放在二级目录中，但也需要同步修改词库设置文件`{方案名称}.dict.yaml`中的词库路径。

#### 后续更新词库
下载更新后的词库文件，覆盖原文件`RIMEDotA2.dict.yaml`即可。

### 更正工具的使用
如果你的rime包含`corrector.lua`，那么可以将我制作的错字错音修正 `lua/corrector.lua` 并入该文件中。
