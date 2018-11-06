# Progress List
- [x] iCloud Photos
- [x] ReStyle IDE
- [x] ConvertICO
- [x] Linmeos Dev
- [x] CydiaUpdates
- [x] BundleID Search
- [x] ConvertICO
- [ ] Google
- [ ] YouTube
- [ ] eBay
- [ ] Amazon
- [ ] PayPal
- [ ] GitHub

# To-Do List
- [ ] Fix various issues on iCloud
- [ ] Finish Google stylesheet
- [X] Add white cursor to ReStyle IDE
- [ ] Fix export UI on ReStyle IDE
- [ ] Fix CSS code editor size bug
- [X] Add highlight colour to editor

# Design Guidelines
## Basic Design Language
The basic design language focuses on a dark interface with a touch of color and motion to signify buttons and actions when pressed or hovered.
The most basic background color should have a hex value of:
```
#292C30
```
White text will be used primarily however using text with an RGBA value can also be used in order to create darker text. In this format you can vary the alpha value in order to get the desired gray. For example, an element which should not be the main focus of the user could have a alpha of 50% eg:
```cs
  rgba(255,255,255,0.5)
```
Links should be used a light blue color with the following hex value. The hover effect can be created by applying a 50% alpha.
```
#2a90fc
```

## Big Box
This one is used in order to hold content. Don't use it too much. Large titles should be placed outside the box.
```css
{
  background: #2F3439;
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.25);
  text-align: left;
  color: white;
  border-radius: 25px;
  padding: 15px;
  line-height: 1.6;
  border-style: solid;
  border-color: rgba(255, 255, 255, 0.03);
  border-width: 2px;
}
```

## Buttons
This is a button, the rest is pretty self-explanatory. Links are NOT equal to buttons. Use wisely!
```css
{
  background: linear-gradient(to right, #55B49D , #2B7DCA);
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.25);
  text-align: center;
  font-family: "SF Pro Display";
  border-radius: 25px;
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 15px;
  padding-right: 15px;
  color:white;
  font-size: 20px;
  -webkit-transition: padding 0.5s ease; /*For Safari*/
  transition: padding 0.25s ease;
  transition: 0.25s;
  border: none;
}
```
Don't forget a fancy hover effect!
```css
:hover {
  filter: hue-rotate(90deg);
  font-size: 22px;
  padding-left: 9px;
  padding-right: 9px;
}
```

## Search Boxes
These can also be used for drop-downs or checkboxes.
```css
{
  background: rgba(200, 200, 255, 0.2) ;
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.25);
  text-align: left;
  font-family: "SF Pro Display";
  border-radius: 25px;
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 15px;
  padding-right: 15px;
  color:white;
  font-size: 20px;
  border: none;
  margin-right: 5px;
  border-style: solid;
  border-color: rgba(255, 255, 255, 0.05);
  border-width: 2px;
}
```
Again, don't forget the hover effect!
```css
:hover {
  background: linear-gradient(to right, rgba(149,136,213,0.4) , rgba(171,89,147,0.4));
}
```

## Scroll Bars
Title says it all. If neccesary here is the code for a custom scrollbar. The classes may need to be changed for a specific element.
```css
::-webkit-scrollbar {
  width: 9px;
  height: 9px;
}
::-webkit-scrollbar-track {
    background: rgba(255,255,255,0.08);
    border-radius: 10px;
}
::-webkit-scrollbar-thumb {
    background: rgba(255,255,255,0.20);
    border-radius: 10px;
}
::-webkit-scrollbar-thumb:hover {
    background: rgba(255,255,255,0.25);;
}
```
