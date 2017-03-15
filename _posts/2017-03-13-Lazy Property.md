---
title: Lazy Property
updated: 2017-03-13 21:45
layout: post
author: Yoon
category: Swift 3.0
tags: 
- Swift
- iOS
- Lazy Property

---


### Swift lazy Property

호출이 있어야 값을 초기화하는 프로퍼티

키워드로 lazy var로 사용한다.

~~~ swift
struct lazyCoordinatePoint {
    var x: Int = 0
    var y : Int = 0
}

class lazyPosition {
    lazy var point : lazyCoordinatePoint = lazyCoordinatePoint()
    let name : String
    
    init(name : String) {
        self.name = name
    }
}


let lazyYsPosition : lazyPosition = lazyPosition(name: "윤영석")

print(lazyYsPosition.point) // X:0, Y:0
~~~

