# HigherScript

HigherScript is a  python interpreter that reads python funtion names ect from a file name, IN alphabetical order. it then reads the file content, and again sorts the content of the files by alphabetics. the pairs of funtion and funtion content in each row is executed together.

# Order

We use [dconc's ASCII order](https://www.dconc.gov/home/showpublisheddocument?id=1481) for sorting. `! ” # $ % & ' () * + , - ./ 0 1 2 3 4 5 6 7 8 9 :;< = >? @ A B C D E F G H I J K L M N O P Q R S T U V W X Y Z [\] ^ _ ` {|} ~`

# Examples

## Basic Example

## Error -> Error Resolution

```
.
├── stringofburgers
│   └── = "Burger"
└── print
    └── (stringofburgers)
```
Results in a error due to a variable being called before its decleration. in this case, its interpreted as

```
.
├── print
│   └── (stringofburgers)
└── strinngofburgers
    └── = "Burger"
```
now, the obvious fix is renaming `stringofburgers` to something that comes before print like `astringofburgers`, but `()` comes before `=` in the higherarcy. I spent a long time thinking long and hard after this example what I was doing with my life and about what I could do to make it work. I eventually came to the realization that it \*cant\* work and thats the wonderful thing. **you can't use variables until proven otherwise**. thank you dconc, very cool.