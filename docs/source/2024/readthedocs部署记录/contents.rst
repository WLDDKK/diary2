read the docs 部署记录【排雷向】
==================================

部署坑
########

* 项目文件目录下".readthedocs.yaml"里面的build os 只准填(ubuntu-20.04, ubuntu-22.04, ubuntu-lts-latest),但是我填了windows10

  参考文档:"https://docs.readthedocs.io/en/stable/config-file/v2.html"

* 想用md语法,而不是rst语法写文章,于是引用\ **recommonmark**\模块。但是部署的时候报错,显示在conf.py里有但是找不到

  “Extension error:
     Could not import extension recommonmark (exception: No module named 'recommonmark')”

  \ **做法**\：直接删。