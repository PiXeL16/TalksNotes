# Keeping Designers Happy Via Enums
[Talk URL](https://realm.io/news/slug-patrick-reynolds-keeping-designers-happy-enums/)
-----

* Enums allows you to maintain consistency.
* Use a `Stylesheet.swift` to structure UICode like fonts, colors, etc

```
enum Colors{
  case White

  car color:UIColor{
    switch self{
      case White: return UIColor.white()
    }
  }
}

Colors.White.color
```

* Use the same StyleSheet struct to `prepare` the different UI elements, like cells and other View Controllers
For example


```
override func awakeFromNib(){
  super.awakeFromNib()
  StyleSheet.prepare(self)
}

//In StyleSheet.swift
static func prepare(cell: TestTableViewCell){
  cell.backgroundColor = Color.White.color
}
```

* (Note) Think how to make the Stylesheet not all bloated. Probably Extensions?
