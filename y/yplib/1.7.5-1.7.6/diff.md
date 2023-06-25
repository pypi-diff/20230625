# Comparing `tmp/yplib-1.7.5.tar.gz` & `tmp/yplib-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.5.tar", last modified: Sun Jun 25 08:09:42 2023, max compression
+gzip compressed data, was "dist\yplib-1.7.6.tar", last modified: Sun Jun 25 08:42:40 2023, max compression
```

## Comparing `yplib-1.7.5.tar` & `yplib-1.7.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:09:42.342840 yplib-1.7.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-25 08:09:42.342662 yplib-1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 08:09:42.343290 yplib-1.7.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-25 08:09:25.000000 yplib-1.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:09:42.339069 yplib-1.7.5/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    11533 2023-06-25 06:52:51.000000 yplib-1.7.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.7.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.5/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.5/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.5/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:09:42.341588 yplib-1.7.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 08:09:42.000000 yplib-1.7.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 08:42:40.330376 yplib-1.7.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-25 08:42:40.329374 yplib-1.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 08:42:40.330433 yplib-1.7.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-25 08:42:37.000000 yplib-1.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:42:40.326531 yplib-1.7.6/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11632 2023-06-25 08:42:27.000000 yplib-1.7.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8270 2023-06-25 08:40:25.000000 yplib-1.7.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.6/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.6/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.6/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:42:40.329053 yplib-1.7.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-25 08:42:40.000000 yplib-1.7.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-25 08:42:40.000000 yplib-1.7.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 08:42:40.000000 yplib-1.7.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 08:42:40.000000 yplib-1.7.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.5/LICENSE` & `yplib-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.5/setup.py` & `yplib-1.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.5",
+  version="1.7.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.5/yplib/chart.py` & `yplib-1.7.6/yplib/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from yplib.chart_html import *
 from yplib.index import *
 
 
 # 将 html 中的占位符 替换成数据
 # 并且 导出 生成后的 html 文件
-def insert_data_to_chart(html_data='',
+def insert_data_to_chart(html_data,
                          name=None,
                          x_list=None,
                          y_list=None,
                          legend=None,
                          series=None,
                          smooth=0):
     p_list = [
         'chart_name', 'name', 'x_list', 'y_list', 'legend', 'series', 'smooth'
     ]
     p_data_list = [
         name, name, x_list, y_list, legend, series, smooth
     ]
-    for index in range(len(p_list)):
-        one_p = p_list[index]
-        one_data = p_data_list[index]
-        if one_data is None:
-            continue
-        one_p = f'-{one_p}-'
-        if one_p in html_data:
-            html_data = html_data.replace(one_p, str(one_data))
-    to_txt(data_list=[html_data],
+    h_r = []
+    for html_line in html_data:
+        for index in range(len(p_list)):
+            one_p = p_list[index]
+            one_data = p_data_list[index]
+            if one_data is None:
+                continue
+            one_p = f'-{one_p}-'
+            if one_p in html_line:
+                html_line = html_line.replace(one_p, str(one_data))
+        h_r.append(html_line)
+    to_txt(data_list=h_r,
            file_name=str(name),
            file_path='html',
            fixed_name=False,
            suffix='.html')
     # current_path = os.path.abspath(__file__)
     # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
```

### Comparing `yplib-1.7.5/yplib/chart_html.py` & `yplib-1.7.6/yplib/chart_html.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,248 +1,248 @@
 # 使用 echarts 的基本图表
-def chart_html(option=''):
-    s = '<!DOCTYPE html>' \
-        '<html lang="zh-CN" style="height: 100%">' \
-        '<head>' \
-        '    <meta charset="utf-8">' \
-        '</head>' \
-        '<body style="height: 100%; margin: 0">' \
-        '<div id="container" style="height: 100%"></div>' \
-        '<script type="text/javascript" src="https://fastly.jsdelivr.net/npm/echarts@5.4.2/dist/echarts.min.js"></script>' \
-        '<script type="text/javascript">' \
-        '    var dom = document.getElementById("container");' \
-        '    var myChart = echarts.init(dom, null, {' \
-        '        renderer: "canvas",' \
-        '        useDirtyRect: false,' \
-        '    });' \
-        '    var app = {};' \
-        '    var option = -option-;' \
-        '    if (option && typeof option === "object") {' \
-        '        myChart.setOption(option);' \
-        '    }' \
-        '    window.addEventListener("resize", myChart.resize);' \
-        '</script>' \
-        '</body>' \
-        '</html>' \
-        ''
-    return s.replace('-option-', option)
+def chart_html(option):
+    s = ['<!DOCTYPE html>',
+         '<html lang="zh-CN" style="height: 100%">',
+         '<head>',
+         '    <meta charset="utf-8">',
+         '</head>',
+         '<body style="height: 100%; margin: 0">',
+         '<div id="container" style="height: 100%"></div>',
+         '<script type="text/javascript" src="https://fastly.jsdelivr.net/npm/echarts@5.4.2/dist/echarts.min.js"></script>',
+         '<script type="text/javascript">',
+         '    var dom = document.getElementById("container");',
+         '    var myChart = echarts.init(dom, null, {',
+         '        renderer: "canvas",',
+         '        useDirtyRect: false,',
+         '    });',
+         '    var app = {};',
+         '    var option = -option-;',
+         '    if (option && typeof option === "object") {',
+         '        myChart.setOption(option);',
+         '    }',
+         '    window.addEventListener("resize", myChart.resize);',
+         '</script>',
+         '</body>',
+         '</html>',
+         '']
+    return list(map(lambda x: x.replace('-option-', '\n'.join(option)), s))
 
 
 # 折线图的 html 模板代码
 def line_stack_html():
-    option = '{' \
-             '    title: {' \
-             '        text: "-chart_name-",' \
-             '    },' \
-             '    tooltip: {' \
-             '        trigger: "axis",' \
-             '    },' \
-             '    dataZoom: [' \
-             '        {' \
-             '            show: true,' \
-             '            realtime: true,' \
-             '        },' \
-             '        {' \
-             '            type: "inside",' \
-             '            realtime: true,' \
-             '        },' \
-             '    ],' \
-             '    grid: {' \
-             '        left: "30px",' \
-             '        right: "40px",' \
-             '        bottom: "80px",' \
-             '        containLabel: true,' \
-             '    },' \
-             '    toolbox: {' \
-             '        feature: {' \
-             '            saveAsImage: {pixelRatio:5},' \
-             '        },' \
-             '    },' \
-             '    yAxis: {' \
-             '        type: "value",' \
-             '    },' \
-             '    xAxis: {' \
-             '        type: "category",' \
-             '        boundaryGap: false,' \
-             '        data: -x_list-,' \
-             '    },' \
-             '    legend: {' \
-             '        -legend-,' \
-             '    },' \
-             '    series: -series-,' \
-             '}'
+    option = ['{',
+              '    title: {',
+              '        text: "-chart_name-",',
+              '    },',
+              '    tooltip: {',
+              '        trigger: "axis",',
+              '    },',
+              '    dataZoom: [',
+              '        {',
+              '            show: true,',
+              '            realtime: true,',
+              '        },',
+              '        {',
+              '            type: "inside",',
+              '            realtime: true,',
+              '        },',
+              '    ],',
+              '    grid: {',
+              '        left: "30px",',
+              '        right: "40px",',
+              '        bottom: "80px",',
+              '        containLabel: true,',
+              '    },',
+              '    toolbox: {',
+              '        feature: {',
+              '            saveAsImage: {pixelRatio:5},',
+              '        },',
+              '    },',
+              '    yAxis: {',
+              '        type: "value",',
+              '    },',
+              '    xAxis: {',
+              '        type: "category",',
+              '        boundaryGap: false,',
+              '        data: -x_list-,',
+              '    },',
+              '    legend: {',
+              '        -legend-,',
+              '    },',
+              '    series: -series-,',
+              '}']
     return chart_html(option)
 
 
 # 折线图的 html 模板代码
 def line_area_html():
-    option = '{' \
-             '  tooltip: {' \
-             '    trigger: "axis",' \
-             '  },' \
-             '  title: {' \
-             '    text: "-chart_name-"' \
-             '  },' \
-             '  toolbox: {' \
-             '    feature: {' \
-             '      saveAsImage: {pixelRatio:5}' \
-             '    }' \
-             '  },' \
-             '    grid: {' \
-             '        left: "30px",' \
-             '        right: "40px",' \
-             '        bottom: "80px",' \
-             '        containLabel: true,' \
-             '    },' \
-             '  xAxis: {' \
-             '    type: "category",' \
-             '    boundaryGap: false,' \
-             '    data: -x_list-' \
-             '  },' \
-             '  yAxis: {' \
-             '    type: "value",' \
-             '  },' \
-             '    dataZoom: [' \
-             '        {' \
-             '            show: true,' \
-             '            realtime: true,' \
-             '        },' \
-             '        {' \
-             '            type: "inside",' \
-             '            realtime: true,' \
-             '        },' \
-             '    ],' \
-             '  series: [' \
-             '    {' \
-             '      type: "line",' \
-             '      symbol: "none",' \
-             '      smooth: -smooth-,' \
-             '      sampling: "lttb",' \
-             '      itemStyle: {' \
-             '        color: "rgb(255, 70, 131)"' \
-             '      },' \
-             '      areaStyle: {' \
-             '        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [' \
-             '          {' \
-             '            offset: 0,' \
-             '            color: "rgb(255, 158, 68)"' \
-             '          },' \
-             '          {' \
-             '            offset: 1,' \
-             '            color: "rgb(255, 70, 131)"' \
-             '          }' \
-             '        ])' \
-             '      },' \
-             '      data: -y_list-' \
-             '    }' \
-             '  ]' \
-             '}'
+    option = ['{',
+              '  tooltip: {',
+              '    trigger: "axis",',
+              '  },',
+              '  title: {',
+              '    text: "-chart_name-"',
+              '  },',
+              '  toolbox: {',
+              '    feature: {',
+              '      saveAsImage: {pixelRatio:5}',
+              '    }',
+              '  },',
+              '    grid: {',
+              '        left: "30px",',
+              '        right: "40px",',
+              '        bottom: "80px",',
+              '        containLabel: true,',
+              '    },',
+              '  xAxis: {',
+              '    type: "category",',
+              '    boundaryGap: false,',
+              '    data: -x_list-',
+              '  },',
+              '  yAxis: {',
+              '    type: "value",',
+              '  },',
+              '    dataZoom: [',
+              '        {',
+              '            show: true,',
+              '            realtime: true,',
+              '        },',
+              '        {',
+              '            type: "inside",',
+              '            realtime: true,',
+              '        },',
+              '    ],',
+              '  series: [',
+              '    {',
+              '      type: "line",',
+              '      symbol: "none",',
+              '      smooth: -smooth-,',
+              '      sampling: "lttb",',
+              '      itemStyle: {',
+              '        color: "rgb(255, 70, 131)"',
+              '      },',
+              '      areaStyle: {',
+              '        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [',
+              '          {',
+              '            offset: 0,',
+              '            color: "rgb(255, 158, 68)"',
+              '          },',
+              '          {',
+              '            offset: 1,',
+              '            color: "rgb(255, 70, 131)"',
+              '          }',
+              '        ])',
+              '      },',
+              '      data: -y_list-',
+              '    }',
+              '  ]',
+              '}']
     return chart_html(option)
 
 
 # 饼图的 html 模板代码
 def pie_html():
-    option = '{' \
-             '  title: {' \
-             '    text: "-chart_name-",' \
-             '    left: 10' \
-             '  },' \
-             '  tooltip: {' \
-             '    trigger: "item"' \
-             '  },' \
-             '    toolbox: {' \
-             '        feature: {' \
-             '            saveAsImage: {pixelRatio:5},' \
-             '        },' \
-             '    },' \
-             '  legend: {' \
-             '    top: "5%",' \
-             '    left: "center"' \
-             '  },' \
-             '  series: [' \
-             '    {' \
-             '      name: "-chart_name-",' \
-             '      type: "pie",' \
-             '      radius: ["30%", "70%"],' \
-             '      itemStyle: {' \
-             '        borderRadius: 10,' \
-             '        borderColor: "#fff",' \
-             '        borderWidth: 1' \
-             '      },' \
-             '      emphasis: {' \
-             '        label: {' \
-             '          show: true,' \
-             '          fontSize: 30,' \
-             '          fontWeight: "bold"' \
-             '        }' \
-             '      },' \
-             '      labelLine: {' \
-             '        show: true' \
-             '      },' \
-             '      data: -x_list-' \
-             '    }' \
-             '  ]' \
-             '}'
+    option = ['{',
+              '  title: {',
+              '    text: "-chart_name-",',
+              '    left: 10',
+              '  },',
+              '  tooltip: {',
+              '    trigger: "item"',
+              '  },',
+              '    toolbox: {',
+              '        feature: {',
+              '            saveAsImage: {pixelRatio:5},',
+              '        },',
+              '    },',
+              '  legend: {',
+              '    top: "5%",',
+              '    left: "center"',
+              '  },',
+              '  series: [',
+              '    {',
+              '      name: "-chart_name-",',
+              '      type: "pie",',
+              '      radius: ["30%", "70%"],',
+              '      itemStyle: {',
+              '        borderRadius: 10,',
+              '        borderColor: "#fff",',
+              '        borderWidth: 1',
+              '      },',
+              '      emphasis: {',
+              '        label: {',
+              '          show: true,',
+              '          fontSize: 30,',
+              '          fontWeight: "bold"',
+              '        }',
+              '      },',
+              '      labelLine: {',
+              '        show: true',
+              '      },',
+              '      data: -x_list-',
+              '    }',
+              '  ]',
+              '}']
     return chart_html(option)
 
 
 # 柱状的 html 模板代码
 def bar_html():
-    option = '{' \
-             '  title: {' \
-             '    text: "-chart_name-",' \
-             '    left: 10' \
-             '  },' \
-             '  toolbox: {' \
-             '    feature: {' \
-             '      dataZoom: {' \
-             '        yAxisIndex: false' \
-             '      },' \
-             '      saveAsImage: {' \
-             '        pixelRatio: 5' \
-             '      }' \
-             '    }' \
-             '  },' \
-             '  tooltip: {' \
-             '    trigger: "axis",' \
-             '    axisPointer: {' \
-             '      type: "shadow"' \
-             '    }' \
-             '  },' \
-             '    grid: {' \
-             '        left: "30px",' \
-             '        right: "40px",' \
-             '        bottom: "80px",' \
-             '        containLabel: true,' \
-             '    },' \
-             '  dataZoom: [' \
-             '    {' \
-             '      type: "inside"' \
-             '    },' \
-             '    {' \
-             '      type: "slider"' \
-             '    }' \
-             '  ],' \
-             '  xAxis: {' \
-             '    data: -x_list-,' \
-             '    silent: false,' \
-             '    splitLine: {' \
-             '      show: false' \
-             '    },' \
-             '    splitArea: {' \
-             '      show: false' \
-             '    }' \
-             '  },' \
-             '  yAxis: {' \
-             '    splitArea: {' \
-             '      show: false' \
-             '    }' \
-             '  },' \
-             '  series: [' \
-             '    {' \
-             '      type: "bar",' \
-             '      data: -y_list-,' \
-             '      large: true' \
-             '    }' \
-             '  ]' \
-             '}'
+    option = ['{',
+              '  title: {',
+              '    text: "-chart_name-",',
+              '    left: 10',
+              '  },',
+              '  toolbox: {',
+              '    feature: {',
+              '      dataZoom: {',
+              '        yAxisIndex: false',
+              '      },',
+              '      saveAsImage: {',
+              '        pixelRatio: 5',
+              '      }',
+              '    }',
+              '  },',
+              '  tooltip: {',
+              '    trigger: "axis",',
+              '    axisPointer: {',
+              '      type: "shadow"',
+              '    }',
+              '  },',
+              '    grid: {',
+              '        left: "30px",',
+              '        right: "40px",',
+              '        bottom: "80px",',
+              '        containLabel: true,',
+              '    },',
+              '  dataZoom: [',
+              '    {',
+              '      type: "inside"',
+              '    },',
+              '    {',
+              '      type: "slider"',
+              '    }',
+              '  ],',
+              '  xAxis: {',
+              '    data: -x_list-,',
+              '    silent: false,',
+              '    splitLine: {',
+              '      show: false',
+              '    },',
+              '    splitArea: {',
+              '      show: false',
+              '    }',
+              '  },',
+              '  yAxis: {',
+              '    splitArea: {',
+              '      show: false',
+              '    }',
+              '  },',
+              '  series: [',
+              '    {',
+              '      type: "bar",',
+              '      data: -y_list-,',
+              '      large: true',
+              '    }',
+              '  ]',
+              '}']
     return chart_html(option)
```

### Comparing `yplib-1.7.5/yplib/db.py` & `yplib-1.7.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.5/yplib/file.py` & `yplib-1.7.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.5/yplib/http_util.py` & `yplib-1.7.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.5/yplib/index.py` & `yplib-1.7.6/yplib/index.py`

 * *Files identical despite different names*

