# 通讯录样式的边栏字母导航

## 简介
创建一个通讯录边栏样式的字母导航

![瀵艰埅](https://github.com/coolzjy/alphabet-sidenav/raw/gh-pages/contacts.jpg)

## DEMO
请扫描二维码在移动设备上查看

![DEMO](http://zjy.name/lab/alphabet-nav/code.png)

## 浣跨敤
#### 1.妯″潡鍖栬皟鐢�
浣跨敤 browserify 鎴� seajs 绛夊伐鍏凤紝寮曞叆alphabetnav

```javascript
var alphabetNav = require('alphabetnav');
alphabetNav.alphabetNav("attrName");
```

#### 2.浣跨敤`script`鏍囩鍏ㄥ眬寮曠敤

```html
<script type="text/javascript" src="script/alphabetNav.js"></script>
<script type="text/javascript">
	alphabetNav("attrName");
</script>
```

#### 3.鏂规硶璋冪敤1(鎺ㄨ崘)

```javascript
alphabetNav("attrName",{options})
```

鍏朵腑锛宎ttrName 涓哄睘鎬у悕锛宱ptions 涓洪厤缃」銆傚厓绱犲睘鎬у悕鐨勫搴斿睘鎬у�煎皢浣滀负瀵艰埅鏄剧ず鍐呭銆傝璋冪敤鏂瑰紡涓� URL Hash 璺宠浆鐗规�т笉鍙敤銆�

DEMO:
```html
<section nav="A">
<section nav="B">
鈥︹��
<section nav="Z">

<script type="text/javascript">
alphabet("nav");
</script>
```

#### 3.鏂规硶璋冪敤2

```javascript
alphabetNav([navItem],{options})
```

鍏朵腑锛宯avItem 涓哄璞℃暟缁勶紝瀵硅薄鍖呮嫭 display 鍜� id 涓や釜灞炴�э紝display 涓哄鑸樉绀哄悕绉帮紝id 涓哄搴旈〉闈㈤敋鐐瑰悕绉般��

DEMO:
```html
<section id="a">
<section id="b">
<section id="c">

<script type="text/javascript">
alphabet([
		{display:"A", id:"a"},
		{display:"B", id:"b"},
		{display:"C", id:"c"}
		]);
</script>
```

### 閰嶇疆椤�
options 鍙�夐厤缃寘鎷細
+ top锛氭暟瀛楁垨瀛楃涓诧紝璁剧疆杈规爮鐨� top 灞炴�с��
+ bottom锛氭暟瀛楁垨瀛楃涓诧紝璁剧疆杈规爮鐨� bottom 灞炴�э紝top 鍜� bottom 鍧囨病鏈夐厤缃椂锛宻lideNav 灏嗗眳涓樉绀恒��
+ showIndicator锛氬竷灏斿瀷锛岄粯璁ゅ�� true锛岃缃槸鍚︽樉绀哄瓧姣嶆寚绀哄櫒銆�
+ useHash锛氬竷灏斿瀷锛岄粯璁ゅ�� false锛屾槸鍚︿娇鐢� URLHash 杩涜璺宠浆銆傛敞鎰忎娇鐢� URLHash 杩涜璺宠浆鏃讹紝鍙湪 URLHash 鏀瑰彉鏃惰烦杞墠浼氬彂鐢燂紝杩欏皢瀵艰嚧鏌愪簺鎯呭喌涓嬩笉鑳借烦杞埌姝ｇ‘浣嶇疆銆�