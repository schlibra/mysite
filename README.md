# MySite
MySite ver.0.0.1

# 安装

1. 将文件解压到服务器相应目录
2. /config.yml.example 改成 /config.yml，并按照您的需求修改
3. 运行 python ./configure.py

# 更新

1. 新版本覆盖旧版本（保留配置文件和你原来的数据）
2. 修改配置文件，将您的配置文件适配新版本。
3. 运行 python ./configure.py

## 最新配置文件
```
php_base: ''
html_base: ''
site_name: ''
master_name: ''
site_name_h2: ''
home_name: ''
avatar: ''

blog: 'xxx'
docs_site: 'xxx'
relax: 'xxx'

pages:
  local:
    - '/home'
    - '/goto'
  local_img:
    - '"._HTML_RES_."/icon/site/home.png'
    - '"._HTML_RES_."/icon/site/goto.png'
  local_title:
    - '小屋'
    - '去往'
  other:
    - 'xxx'
  other_img:
    - '"._HTML_RES_."/icon/site/blog.png'
  other_title:
    - '博客'
  home_local:
    - 'search'
    - 'time'
    - 'projects'
    - 'videos'
  home_local_title:
    - '搜索'
    - '时间'
    - '项目'
    - '视频'
  home_local_intro:
    - 'search'
    - 'time'
    - 'projects'
    - 'videos'
  home_other:
    - 'xxx'
    - 'xxx'
  home_other_title:
    - '文档'
    - '休闲'
  home_other_intro:
    - 'docs'
    - 'relax'
  
# Links in bottom
# 1. github
# 2. gitee
# 3. bilibili
# 4. zhihu
# 5. rss
# 6. twitter
# 7. youtube
links:
  onoff:
# If you have, input the addresses. If not, input 'no'.
    - 'no'
    - 'no'
    - 'no'
    - 'no'
    - 'no'
    - 'no'
    - 'no'
  logos:
    - '"._HTML_RES_."/icon/connect/github.webp'
    - 'https://gitee.com/favicon.ico'
    - 'https://www.bilibili.com/favicon.ico'
    - 'https://zhihu.com/favicon.ico'
    - '"._HTML_RES_."/icon/connect/rss.jpg'
    - '"._HTML_RES_."/icon/connect/twitter.jpeg'
    - '"._HTML_RES_."/icon/connect/youtube.jpeg'

goto:
  title:
    - '世界上第一个网站'
    - 'WCC实验室官网'
    - 'Github'
  link:
    - 'http://info.cern.ch'
    - 'https://wcc.group'
    - 'https://github.com'
  intro:
    - 'info.cern.ch'
    - 'wcc.group'
    - 'Build software better, together.'

site_birthday: '07/21/2021'

projects:
  name:
    - 'project'
  link:
    - 'disabled'
  img:
    - 'xxx'
  intro:
    - 'xxx'
  opensrc:
    - 'BSD-3 Clause'
  github:
    - 'https://github.com/xxx/xxx'
  gitee:
    - 'disabled'
  download:
    - 'disabled'

videos:
  title:
    - '元首的愤怒'
    - '歌唱动荡的青春 红场千人大合唱版本'
  img:
    - 'none'
    - 'none'
  intro:
    - '元首的愤怒 气死偶嘞'
    - '歌唱动荡的青春 红场千人大合唱版本 哈利洛夫指挥'
  link:
    - 'disabled'
    - 'disabled'
  bilibili:
    - 'aid=22905&bvid=BV1Hx411c7iM&cid=37878'
    - 'aid=37278610&bvid=BV1tt411D7NA&cid=65516888'
    
main_color:
  light: '#95afff'
  dark: '#051f7f'

aplayer:
  enable: true
  default_cover: '"._RES_."/img/aplayer/default.png'

enable_travelling: true

# Comment System
# like waline
comment: xxx

background:
  light_color: '#95afff'
  dark_color: '#051f7f'
  enable_image: false
  pictures_group: 'xxx'
  number: 10

head:
  - <meta charset="utf-8">
  - <meta name="viewport" content="width=device-width,initial-scale=1">
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/header.css" type="text/css"/>
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/img.css" type="text/css"/>
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/style.css" type="text/css"/>
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/style_dark.css" type="text/css"/>
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/side.css" type="text/css"/>
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/footer.css" type="text/css"/>
  - <link rel="stylesheet" href="'._HTML_RES_.'/css/APlayer.min.css" type="text/css"/>
  - <script src="'._HTML_RES_.'/js/jquery-3.4.1.min.js" type="text/javascript"></script>
  - <script src="'._HTML_RES_.'/js/APlayer.min.js" type="text/javascript"></script>

include_func:
  - _RES_.'/conf/head.php'
  - _RES_.'/conf/pages.php'
  - _RES_.'/conf/goto.php'
  - _RES_.'/conf/videos.php'
  - _RES_.'/conf/links.php'
  - _RES_.'/conf/pictures.php'
  - _RES_.'/conf/projects.php'
  - _RES_.'/web/version.php'
  - _DARKMODE_
  - _PAGE_BG_
  
files_const:
  php_res_dir: $_BASE_.'/res'
  html_res_dir: _HTML_BASE_.'/res'
  include_dir: _RES_.'/conf/include.php'
  pages:
    header: _RES_.'/web/header.php'         # _PAGE_HEADER_
    footer: _RES_.'/web/footer.php'         # _PAGE_FOOTER_
    bg: _RES_.'/web/bg.php'                 # _PAGE_BG_
    aplayer: _RES_.'/web/aplayer.php'       # _PAGE_APLAYER_
    side: _RES_.'/web/side.php'             # _PAGE_SIDE_
  darkmode: _RES_.'/web/darkmode.php'
  comment:
    xxx: _RES_.'/web/comment_none.php'
    waline: _RES_.'/web/waline.php'
```

# 更新

- 0.0.1: 第一个版本
- 0.0.2: 修补了一些bug
- 0.0.3：支持yaml配置文件 
 
