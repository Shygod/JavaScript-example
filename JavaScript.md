JavaScript
===

HTML-DOM-Method
---

#### *getElementById()方法*

> 搜尋元素id屬性值<br />

* 範例:使用 **getElementById()** 方法，修改元素的文字內容

```HTML
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <title>JavaScript-HTML-DOM-getElementById-method</title>
    </head>
    <body>
        <p id="demo"></p>
        <script>
            // 從頁面上搜尋id屬性值為demo的元素
            var demo = document.getElementById("demo");
            demo.innerHTML = "Hello World!";
        </script>
    </body>
</html>
```

#### *getElementsByTagName()方法*

> 從HTML頁面上搜尋所有指定的標籤名稱

* 範例:使用 **getElementsByTagName()** 方法，修改搜尋到的所有元素文字內容

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <title>JavaScript-HTML-DOM-getElementsByTagName-method</title>
    </head>
    <body>
        <p>這是第一個段落</p>
        <p>這是第二個段落</p>
        <p>這是第三個段落</p>
        <div>
            <p>這是第四個段落</p>
        </div>
        <script>
            // 搜尋頁面上所有<p>元素
            var paragraph = document.getElementsByTagName('p');

            // 使用迴圈訪問所有元素，並將內容修改
            for(let i=0; i<paragraph.length; i++) {
                paragraph[i].innerHTML = "這是索引值:" + i;
            }
        </script>
    </body>
</html>
```

#### *getElementsByClassName()方法*

> 從HTML頁面上搜尋所有指定class屬性值的元素

* 範例:使用 **getElementsByClassName()** 方法，修改搜尋到的所有元素文字內容

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <title>JavaScript-HTML-DOM-getElementsByClassName-method</title>
    </head>
    <body>
        <h1 class="love">屬性值:love</h1>
        <p class="love">屬性值:love</p>
        <span class="love">屬性值:love</span><br />
        <em class="love">屬性值:love</em><br />
        <strong class="honey">屬性值:honey</strong><br />
        <script>
            // 從頁面上搜尋所有class屬性值為love的元素
            var love = document.getElementsByClassName('love');
            // 使用迴圈訪問所有元素，並將內容修改
            for(let i=0; i<love.length; i++) {
                love[i].innerHTML = "這是索引值:" + i;
            }
        </script>
    </body>
</html>
```

#### *createElement()方法*

> 從JavaScript新增元素節點

* 範例:使用 **createElement()** 方法，將新增的元素節點插入到頁面上

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <title>JavaScript-HTML-DOM-createElement-method</title>
    </head>
    <body>
        <script>
            // 使用createElement()方法，建立節點
            var new_element = document.createElement('p');
            // 使用createTextNode()方法，建立文字節點
            var txt         = document.createTextNode("這是從JavaScript新增的元素節點");
            // 將建立的文字插入到新增的<p>元素底下
            new_element.appendChild(txt);
            // 將<p>元素插入到頁面上
            document.body.appendChild(new_element);
        </script>
    </body>
</html>
```

#### *createTextNode()方法*

> 從JavaScript新增文字節點

* 範例:使用 **createTextNode()** 方法，將新增的文字節點插入到頁面上指定的元素

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <title>JavaScript-HTML-DOM-createTextNode-method</title>
    </head>
    <body>
        <h1 id="changeText"></h1>
        <script>
            // 搜尋元素將新增的文字節點插入
            var changeText = document.getElementById("changeText");
            var txt        = document.createTextNode("這是從JavaScript新增的文字節點");
            changeText.appendChild(txt);
        </script>
    </body>
</html>
```

HTML-DOM-Attribute
---

HTML-DOM-Event
---

