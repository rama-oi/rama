The idea behind this language is that is separated from any spoken language, so no reserved words for it.

---------------------------
End statement
```
;
```
---------------------------
Variable declaration
> the circle represent how this is dynamic
```
var a = 1;
```
```
● a ← 1;
```

---------------------------
Const declaration
> the square represent how is supossed to be static
```
const black = 0;
```
```
■ black ← 0;
```

---------------------------
Conditions
> Else is basically an empty if
```
if (a == b && b != c) {

} else {

}
```
```
? (a = b && b <> c) {

} ? {

};
```

---------------------------
Input
```
read(a)
```
```
↑(a);
```

---------------------------
Output
```
write("sum: " + 1 + 2);
```
```
↓("sum: {}", 1 + 2);
```

---------------------------
For loop declaration
> the break is an arrow indicating to move forward
```
for c = 1 to 5 {
  if(c == 2 / 5){
    break;
  }
  write(c)
}
```
```
● c ← 1..5
  ? ( c = 2 / 5 ) { → };
  ↓(c);
;
```

---------------------------
While loop declaration
> Technically a for that end up in a condition that will never met
```
var c = 0;
while c < 4 {
  c += 1; 
  write(c)
}
```
```
● c ← 1..? ( 2 = 3 )
  ? c >= 4 { → };
  ↓(c);
;
```

---------------------------
Array declaration
```
var c = array[1,2,3,4,5];
```
```
● c ← 1..5;
```

---------------------------
Array map declaration
```
var c = array[1,2,3,4,5].map(a => a - 5)
```
```
● c ← - 5 \\ 1..5;
```

---------------------------
Array reduce declaration
```
var c = array[1,2,3,4,5].reduce((acc, curr) => acc + curr)
```
```
● c ← + \ 1..5;
```
```
+\ summatory
-\ subtraction
*\ multiplication
/\ division
!\ factorial
```

---------------------------
Array find
```
var current = [1,2,3,4,5].find(a => a == 1);
```
```
● current ← ? ( a = 1 ) \ 1..5;
```

```
var current = [1,2,3,4,5].find(a => a / 5 == 1)
```
```
● current ← ? ( a / 5 = 1 ) \ 1..5;
```

---------------------------
Array items
```
var current = a[5];
```
```
● current ← a[5];
```

---------------------------
Run commands
```
command("ls -a");
```
```
$ls -a;
```

---------------------------
Write into files
```
"hi" >> file.txt
```
```
$"hi" >> file.txt;
```

---------------------------
Comments
> A block of codes that needs to be skip or jump over, the tilde represent a speed bump
```
/*
hi
*/
```
```
~
hi
;
```

---------------------------
Array includes
```
if ([1,2,3,4,5].includes(5)) {
  write(true)
}
```
```
? 5 ∈ 1..5 {
  ↓(true);
};
```

---------------------------
Functions
> the return is a value that is assign back to the function
```
function summatory(a, b){
  return a + b
}
```
```
ƒ summatory ( a, b ) {
  ← a + b;
};
```

---------------------------
Include/import
```
import {summatory as sum} from "./module.rama";
```
```
++ ■ sum ← summatory :: "./module.rama";
```
```
import {summatory} from "./module.rama";
```
```
++ ■ summatory :: "./module.rama";
```
```
import "./module.rama";
```
```
++ "./module.rama";
```

---------------------------
Export/Public
```
pub fn convert(a){
  return a*8;
}
```
```
∀ ƒ convert ( a ) {
  ← a * 8;
};
```

---------------------------
Null/isEmpty
```
if(arr.length == 0) {}
```
```
? arr = ∅ {};
```
