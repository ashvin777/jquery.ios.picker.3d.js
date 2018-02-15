# jquery.ios.picker.3d.js

http://ashvin777.github.io/jquery.ios.picker.3d.js/


ios.picker.js is a dynamic, mobile-friendly jQuery data picker plugin which allows you to quickly select data (such as date, time, city, gender, number, product, and much more) from an iOS style comprehensive picker interface using mouse whee and/or touch swipe. 

How to use it:
1. Include the main style sheet for the iOS data picker.

```
<link href="index.css" rel="stylesheet">
```
2. Create a container to place your data picker.

```
<div id="example-picker"></div>
```
3. Put jQuery JavaScript library and the ios.picker.js script at the bottom of the html page.

```
<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
```
```
<script src="jquery.ios.picker.js"></script>
```
4. Enable the iOS data picker and define your own data in the data array.

```
$("#example-picker").picker({
  data: ['jQuery', 'Script', 'Net', 'AngularJS', 'ReactJS', 'VueJS', 'React Native']
}
```

5. Set the line height.
```
$("#example-picker").picker({
  lineHeight: 50, // default: 30
}
```
```
6. Set pre-seleted item.
$("#example-picker").picker({
  selected: 0
}
```

7. Get and output the user picked item:

```
<div class="output"></div>
```
```
$("#example-picker").picker({
  data: ['jQuery', 'Script', 'Net', 'AngularJS', 'ReactJS', 'VueJS', 'React Native'],
  lineHeight: 30,
  selected: 0
}, function (s) {
  $(".output").html(s);
  $(".example-picker").data("value", s);
});
```
