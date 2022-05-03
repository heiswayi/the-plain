---
layout: post
title: "Constructing a supply chain index"
comments: true
description: "Replicating BOE"
keywords: "dummy content"
---


The Bank of England[^1] has this interesting chart in its Monetary Policy Report:

### Image
<img src="https://raw.githubusercontent.com/zulfadz/zulfadz.github.io/master/pictures/BOE.png" width="400" height="400" />

which turns out to be pretty easy to replicate following the instructions from the footnote. Below is the replication code in eviews:

```javascript
var modularpattern = (function() {
    // your module code goes here
    var sum = 0 ;

    return {
        add:function() {
            sum = sum + 1;
            return sum;
        },
        reset:function() {
            return sum = 0;    
        }  
    }   
}());
alert(modularpattern.add());    // alerts: 1
alert(modularpattern.add());    // alerts: 2
alert(modularpattern.reset());  // alerts: 0
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting.
But let's throw in a <b>tag</b>.
```


<div class="divider"></div>


### Findings


Note that there is another [supply chain index](https://libertystreeteconomics.newyorkfed.org/2022/03/global-supply-chain-pressure-index-march-2022-update/), which is similar, except that it uses more information by allowing for cross-country linkages and more measures of transportation costs.

Footnote:

[^1]: [Monetary Policy Report February 2022](https://www.bankofengland.co.uk/-/media/boe/files/monetary-policy-report/2022/february/monetary-policy-report-february-2022.pdf)





