# JSON 用法：
## Format:
```json
	{
	“key” : value ,
	“key” : value ,
	“key” : [{
		 “key” : value,
		 “key” : value
		 }]
	}
```

JS语法：
```javascript
obj = JSON.parse(data)
data =
	“key”：value，
	“key”：value
data= []
data.push(“key”,value)
JSON.stringify (data)
```

可以用`obj[“key”]`赋值/取值

Java语法：
```java
JsonNode json = Json.parse(data);
Json.get(“key”);
ObjectNode node = Json.newObject();
node.put(“key”,value);
return ok(node);
```







SCALA 模板
```java
Result ok(views.html.xxx.render(input));

```
```scala
CONTENT:content.scala.html
@(input : Type)
@import java.util.Date; var count=0;
@layout(inputForLayout,inputForLayout……) {
	@for( dish <- dishes ) {
		@if(true) {
	<div></div>
		} else {
			<p></p>
		}
}
	<script>
		window.data = “@jsonString”;
	</script>
}


LAYOUT:layout.scala.html

@(inputForLayout:Type,inputForLayout:Type……)(content:Html)

	@content

```




翻译：

`Javascripts`
`lang.coffee`
方法：`switchLan（）`，`getLang（）`,`loadLang()`……
```coffeescript
translation.coffee
“title”
“en” : “Title”
“zh-CN” : “标题”
```

```html
<span class=“lang” title=“title”>empty</span>
<input />
<button>
```

Java：

```java
Lang.java
Lang(“title”).get(“en”);
String lang = Lang.getLang();
Lang.get(“title”,”en”);
```


数据库：
```java
Dish.java:
public static Finder<Integer, Dish> find = new Finder<Integer, Dish>(Integer.class, Dish.class);
access:
Dish dish = Dish.find.byId(id);
Dish dish = Dish.find.where().eq(“name”,name).nq().gt().findUnique();
List<Dish> dish = Dish.find.where().eq(“name”,name).nq().gt().orderBy(“sort”).findList();
```

找到后要检查是否valid
```java
if (dish==null)(或其他)
	return ok(fail message);
```

向后台传数据：

html：
```html
<form action="url " method="post" onsubmit='return ValidateForm(this);'>
<input name=”key” />
</form>
```


ajax:
```coffeescript
$.get
   post

  data: {
“key” : value
“key” : value

}
```

java获取data：
```java
DynamicForm in = Form.form().bindFromRequest();
… = in.get(“key”);
```




CSS规范：
Class命名：“menuMiddleBoxZY” 结尾放名字首字母
