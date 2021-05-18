# Syntax for enhance css

enhance css selector syntax for bulding flow to export animation


## enhance method

rule1: add the dom attribute like 'data-[keyword]=yyy', different 'keyword' means different effect

rule2: if css selector doesn't match any dom elements, system will generate the DOM by css selector.

this css meas "it will generate 3 div in document, and the first div style is 'width:100px;height:100px;transform: translate(100px, 0)' "

```css
.selector[data-length=3] {
  width: 100px;
  height: 100px;
  transform: translate( 100px * $index , 0);
}
```
###  preserve variables

such like "$index", this means runtime preserve variables by different keywrods;


## enhance keywords

### data-length

generate a certain number of div. the number due to the keyword value. like example.


-----

to be continute 2021.5.19
