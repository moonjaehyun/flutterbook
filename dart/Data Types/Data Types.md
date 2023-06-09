## Basics Data Types
/*
대부분의 타입들이 객체로 이루어져 있다
*/
```
void main() {
    String name = "tom";
    bool isPlay = true;
    int age = 10;
    double money = 52.55;
    num x = 12;
    num y = 1.2;
}
```
## Lists
/*
List를 사용하는 2가지 방법
*/
```
void main() {
List numbers = [1, 2, 3];
var number2 = [4, 5, 6];
}
```
/*
List는 collection if와 collection for를 지원한다.
collection if는 List를 만들 때, if를 통해 존재할 수도 안 할 수도 있는 요소를 가지고 만들 수 있다.
void main() {
var giveMeFive = true;
var item = [
1,
2,
3,
if (giveMeFive) 10, // giveMeFive가 true이면 10을 넣음
];
print(item);
}
*/


## String Interpolation

/*
변수 사용하는 방법

$달러 기호를 붙이고 사용할 변수를 적어주면 된다.
만약 무언가를 계산하고 싶다면 ${ } 형태로 적어주면 된다.
*/

void main(){
var name = "tom";
var age = 10;
var greeting = "hello $name, I'm ${age + 5}";
}


## Collection For

Dart는 조건문(if) 및 반복(for)을 사용하여 컬렉션을 구축하는 데 사용할 수 있는 컬렉션 if 및 컬렉션 for도 제공합니다.
```
void main() {
var oldFriends = ["nico", "lynn"];
var newFriends = [
"tom",
"jon",
for (var friend in oldFriends) "❤️ $friend"
];

print(newFriends); // [tom, jon, ❤️ nico, ❤️ lynn]
}
```

## Maps

일반적으로 맵은 key와 value를 연결하는 객체입니다. 키와 값 모두 모든 유형의 객체가 될 수 있습니다. 각 키는 한 번만 발생하지만 동일한 값을 여러 번 사용할 수 있습니다.
```
var gifts = {
// Key: Value
'first': 'partridge',
'second': 'turtledoves',
'fifth': 'golden rings'
};

// Map 생성자를 사용하여 동일한 객체를 만들 수 있습니다.
var gifts2 = Map();
gifts2['first'] = 'partridge';
gifts2['second'] = 'turtledoves';
gifts2['fifth'] = 'golden rings';
```

## Sets

Set에 속한 모든 아이템들이 유니크해야될 때 사용한다.
유니크할 필요가 없다면 List를 사용하면 된다.
```
var halogens = {'fluorine', 'chlorine', 'bromine', 'iodine', 'astatine'};
```
