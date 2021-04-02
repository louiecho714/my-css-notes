# flexbox

## flex container
 
Flex 外容器屬性：

1. display
2. flex-flow
    - flex-direction
    - flex-wrap
3. justify-content
4. align-items

=========================================

* flex direction：設定container中item的排列方向[row,column,row-reverse,column-reverse]
```
flex-direction:row  //main-axis:row,cross-axis:column

flex-direction:column  //main-axis:column,cross-axis:row
```
* justify-content：設定主軸的排序方向

* align-items：設定交叉軸排序方向

* flex-wrap：指會不會分行
```
flex-wrap:wrap //內容物超過邊界，會自動下移一行

flex-wrap:nowrap //內容物會自動壓縮大小，不會換行
```

* flex-flow：(flex-direction+flex-wrap)
```
flex-flow: row wrap //flex-direction:row ,flex-wrap:wrap
flex-flow: column nowrap //flex-direction:column ,flex-wrap:nowrap
```

* align-content：當 flex-wrap:wrap ，且內容物超過一行時，才會生效。使內容物跳脫align-items管理，即忽略align-items的設定。


## flex item

Flex 內元件屬性：

1. flex
    - flex-grow
    - flex-shrink
    - flex-basis
2. order
3. align-self

==============================================

* order：用於調整flex item的排序位置，預設0越小越前面，若數值依樣依據html原始元素排序

* align-self：用於覆寫 container中align-items的設定

* flex-grow：當item 伸長時的倍率0,1,2.....

* flex-shrink：當item 收縮時的倍率0,1,2.....

* flex-basis：設定item於主軸的距離，於flex-direction:row 時為item的寬度，於flex-direction:column 時為item的高度。有可能忽視原本item的高度或寬度。

* flex: (flex-grow+flex-shrink+flex-basis)
```
flex-grow:1;
flex-shrink:0;
flex-basis:auto;

==========上下相同效果========================

flex:1 0 auto;
```