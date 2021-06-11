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
##  preserve variables

such like "$index", this means runtime preserve variables by different keywrods;

## support css selector

### child selector

this selector enable to uniquely determin DOM tree.

```
div > .foo {

}
```

## enhance attribute

### [data-length]

generate a certain number of div. the number due to the keyword value. like example.

### $index

type: number

when generate DOM element, the iterator will pass current index to "$index" in the scope.


-----

to be continute 
