# Tìm hiểu biến trong JavaScript
## Biến là gì
- Biến là "tên biểu tượng" dùng để đại diện cho một giá trị. Và giá trị của biến có thể thay đổi trong chương trình.
- **Biến toàn cục (global variable)** là biến mà có thể truy cập từ bất kỳ nơi nào trong chương trình, bao gồm cả trong các hàm, trong khi biến cục bộ (local variable) chỉ có thể truy cập trong phạm vi cụ thể của một khối mã nhất định, chẳng hạn như một hàm hoặc một khối lệnh.
- **Biến cục bộ (local variable):** là một biến được khai báo và chỉ có thể truy cập trong phạm vi cụ thể của một khối mã nhất định, chẳng hạn như một hàm, một phương thức, hoặc một khối lệnh. Nó không thể được truy cập từ bất kỳ nơi nào bên ngoài phạm vi đó. 

## Cách khai báo biến trong JavaScript
- Cú pháp khai báo biến như sau:
```
let <tên biến>;
```
- Để khai báo nhiều biến, bạn có thể dùng dấu phẩy (,) để ngăn cách các biến trên cùng một dòng:
```
let language = "JavaScript",
  message = "Hello",
  date = "Monday";
```
### Cách thay đổi giá trị của biến số
```
// Khai báo biến và gán giá trị ban đầu
let language = "JavaScript";
console.log(language); // JavaScript
// Thay đổi giá trị của biến
language = "React";
console.log(language); // React
```
### Quy tắc đặt tên biến trong JavaScript
**Quy tắc đặt tên biến trong JavaScript như sau:**
- Bắt đầu bằng chữ cái, dấu gạch dưới (_) hoặc kí tự "đô la" ($).
- Sau kí tự đầu tiên, ngoài những kí tự trên, bạn có thể sử dụng thêm số (0-9).
- Không sử dụng từ khoá và từ dự trữ.
# Tìm hiểu hằng trong JavaScript

## Hằng là gì 
- Trong JavaScript, hằng (constants) là các biến mà giá trị của chúng không thay đổi sau khi được gán. Điều này có nghĩa là sau khi một hằng được khai báo và gán một giá trị cụ thể, giá trị đó không thể thay đổi trong quá trình thực thi của chương trình. Việc sử dụng hằng rất hữu ích khi bạn muốn đảm bảo rằng một giá trị không được thay đổi trong toàn bộ mã nguồn của bạn.
- Trong JavaScript, bạn có thể khai báo hằng bằng cách sử dụng từ khóa const. Ví dụ:
```
const PI = 3.14159;
```

- Trong ví dụ trên, PI là một hằng số với giá trị bằng 3.14159, và giá trị của PI không thể thay đổi trong quá trình thực thi của chương trình.

- Khi bạn cố gắng thay đổi giá trị của một hằng, bạn sẽ nhận được một lỗi (error) trong JavaScript.
```const PI = 3.14159;
PI = 3; // Gây ra lỗi vì bạn không thể gán lại giá trị cho một hằng.
```
# Các kiểu dữ liệu trong JavaScript
- JavaScript có **8 kiểu dữ liệu** cơ bản, trong đó, có **7 kiểu dữ liệu nguyên thủy (boolean, null, undefined, number, BigInt, string, symbol)** và **1 kiểu dữ liệu dạng tham chiếu (object).**
Kiểu dữ liệu nguyên thủy: là kiểu dữ liệu mà giá trị không thể thay đổi được. Đây là kiểu dữ liệu ứng với "level thấp nhất" của ngôn ngữ lập trình.
- Kiểu dữ liệu tham chiếu (object): là tập hợp của các thuộc tính (key) và giá trị (value). Mà số lượng các key có thể thay đổi, giá trị ứng với key cũng có thể thay đổi. Do đó, giá trị của kiểu dữ liệu tham chiếu có thể thay đổi được.
 # Chuyển đổi kiểu dữ liệu trong Javascript
 #### Trong JavaScript, bạn có thể chuyển đổi giữa các kiểu dữ liệu khác nhau bằng một số phương pháp khác nhau. Dưới đây là một số cách thông thường để chuyển đổi kiểu dữ liệu trong JavaScript:
 1. **Chuyển đổi sang số (Number):** Bạn có thể sử dụng hàm `Number() `hoặc toán tử `+` để chuyển đổi sang kiểu dữ liệu số. Ví dụ:
 ```
 let strNumber = "123";
let num = Number(strNumber); // Chuyển đổi chuỗi "123" thành số 123

 ```
 2. **Chuyển đổi sang chuỗi (String):** Bạn có thể sử dụng phương thức `toString()` hoặc toán tử nối chuỗi (`+`) để chuyển đổi sang kiểu dữ liệu chuỗi. Ví dụ:  
 ```
 let num = 123;
let str = num.toString(); // Chuyển đổi số 123 thành chuỗi "123"

 ```
 3. **Chuyển đổi sang mảng (Array):** Bạn có thể sử dụng phương thức Array.from() để chuyển đổi một đối tượng có thể lặp (iterable) thành một mảng. Ví dụ:
```
let iterable = "hello";
let arr = Array.from(iterable); // Chuyển đổi chuỗi "hello" thành mảng ["h", "e", "l", "l", "o"]
```
4. **Chuyển đổi sang boolean (Boolean):** Bạn có thể sử dụng toán tử logic hoặc hàm `Boolean() `để chuyển đổi sang kiểu dữ liệu boolean. Ví dụ:
```
let num = 0;
let bool = Boolean(num); // Chuyển đổi số 0 thành giá trị boolean false
```
# Hàm tương tác với người dùng alert, confirm, prompt
### Trong JavaScript, có ba hàm cơ bản để tương tác với người dùng trên trình duyệt web: alert, confirm, và prompt. Dưới đây là mô tả và cách sử dụng của mỗi hàm:

1. **alert:** Hàm `alert `được sử dụng để hiển thị một thông báo đơn giản tới người dùng trên trình duyệt. Ví dụ:
```
alert("Xin chào! Đây là một thông báo đơn giản.");
```
2. **confirm:** Hàm confirm hiển thị một hộp thoại xác nhận với hai lựa chọn "OK" và "Cancel". Nó trả về `true` nếu người dùng chọn "OK" và `false` nếu họ chọn "Cancel". Ví dụ:
```
let result = confirm("Bạn có chắc chắn muốn thực hiện hành động này không?");
if (result) {
    // Thực hiện hành động khi người dùng chọn "OK"
} else {
    // Thực hiện hành động khi người dùng chọn "Cancel"
}

```
3. **prompt:** Hàm `prompt` hiển thị một hộp thoại yêu cầu người dùng nhập dữ liệu. Nó trả về chuỗi văn bản mà người dùng nhập hoặc `null` nếu họ chọn hủy. Ví dụ:
# Các toán tử trong Javascript


### JavaScript cung cấp một loạt các toán tử để thực hiện các phép tính và các phép so sánh khác nhau. Dưới đây là một số toán tử cơ bản trong JavaScript:

1. Toán tử số học:

- `+` Cộng
- `-` Trừ
- `* `Nhân
- `/` Chia
- `%` Chia lấy dư
- `++` Tăng một đơn vị
- `--` Giảm một đơn vị
2. Toán tử gán:

- `=` Gán giá trị
- `+=` Cộng và gán
- `= `Trừ và gán
- `*=` Nhân và gán
- `/=` Chia và gán
3. Toán tử so sánh:

- `==` So sánh bằng
- `===` So sánh bằng cả về giá trị và kiểu dữ liệu
- `!=` So sánh khác
- `!==` So sánh khác về giá trị hoặc kiểu dữ liệu
- `> `Lớn hơn
- `<` Nhỏ hơn
- `>=` Lớn hơn hoặc bằng
- `<=` Nhỏ hơn hoặc bằng
4. Toán tử logic:

- `&&` Toán tử AND logic
- `||` Toán tử OR logic
- `!` Toán tử NOT logic
5. Toán tử ba ngôi (Conditional):

- condition ? expr1 : expr2 Trả về expr1 nếu condition là true, ngược lại trả về expr2.
6. Toán tử chuỗi:

- Nối chuỗi
7. Toán tử typeof:

- typeof Trả về kiểu dữ liệu của toán hạng.
- Ví dụ, các biểu thức sau đây minh họa cách sử dụng một số toán tử trong JavaScript:
```
let x = 5;
let y = 3;
let z = x + y; // z sẽ là 8

let a = 10;
a += 5; // a sẽ là 15

let b = (x > y) ? "x lớn hơn y" : "x nhỏ hơn hoặc bằng y";

```
# So sánh trong Javascript
1. Toán tử so sánh bằng (`==` và `===`):
- `==`: So sánh giá trị của hai toán hạng, không quan tâm đến kiểu dữ liệu.
- `===`: So sánh cả giá trị và kiểu dữ liệu của hai toán hạng.
- Ví dụ:
```
let x = 5;
let y = '5';

console.log(x == y); // true, vì giá trị giống nhau
console.log(x === y); // false, vì kiểu dữ liệu khác nhau
```
2. Toán tử so sánh khác (`!=` và `!==`):
- `!=`: So sánh nếu hai toán hạng khác nhau về giá trị.
- `!==`: So sánh nếu hai toán hạng khác nhau về giá trị hoặc kiểu dữ liệu.
- Ví dụ :
```
let a = 10;
let b = '10';

console.log(a != b); // false, vì giá trị bằng nhau
console.log(a !== b); // true, vì kiểu dữ liệu khác nhau
```
3. Toán tử so sánh lớn hơn và nhỏ hơn (`>`, `<`, `>=`, `<=`):
- `>:` Lớn hơn
- `<:` Nhỏ hơn
- `>=:` Lớn hơn hoặc bằng
- `<=`: Nhỏ hơn hoặc bằng
```
let m = 7;
let n = 5;

console.log(m > n); // true
console.log(m < n); // false
console.log(m >= n); // true
console.log(m <= n); // false
```
# Toán tử logic trong Javascript
1. Toán tử AND (&&): Toán tử AND trả về true nếu cả hai toán hạng đều đúng và trả về false nếu bất kỳ một toán hạng nào là sai.
```
var a = true;
var b = false;
console.log(a && b); // false
```
2. Toán tử OR (||): Toán tử OR trả về true nếu một trong hai toán hạng là true và trả về false nếu cả hai toán hạng đều là false.
```
var a = true;
var b = false;
console.log(a || b); // true
```
3. Toán tử NOT (!): Toán tử NOT đảo ngược giá trị của toán hạng, trả về true nếu toán hạng là false và ngược lại.
```
var a = true;
console.log(!a); // false
```
# Cấu trúc rẽ nhánh trong Javascript
- Câu lệnh if...else if...else: Câu lệnh này sử dụng khi bạn muốn kiểm tra nhiều điều kiện khác nhau.
```
if (condition1) {
    // Thực hiện mã nếu điều kiện 1 là true
} else if (condition2) {
    // Thực hiện mã nếu điều kiện 2 là true
} else {
    // Thực hiện mã nếu cả hai điều kiện trên đều là false
}
```
- Câu lệnh switch: Câu lệnh switch được sử dụng khi bạn có một số lượng lớn các trường hợp để xử lý.
```
switch (expression) {
    case value1:
        // Thực hiện mã nếu expression là value1
        break;
    case value2:
        // Thực hiện mã nếu expression là value2
        break;
    default:
        // Thực hiện mã nếu không có trường hợp nào khớp
}

```
- Toán tử` ? `cùng với `:` được sử dụng để tạo điều kiện ngắn gọn trong JavaScript, còn được gọi là toán tử ba ngôi. Đây là cách cấu trúc chung của nó:
```
condition ? expr1 : expr2
```
- Nó hoạt động theo cách sau: nếu điều kiện là true, toán tử trả về expr1; nếu điều kiện là false, toán tử trả về expr2. Đây là một cách rất tiện lợi để thay thế cho các cấu trúc if...else đơn giản.
# Toán tử ?? trong JavaScript
1. Toán tử ?? (Nullish Coalescing Operator): Toán tử ?? được sử dụng để xác định giá trị mặc định cho một biến nếu giá trị ban đầu là null hoặc undefined. Nó trả về giá trị bên phải nếu giá trị bên trái là null hoặc undefined; ngược lại, nó trả về giá trị bên trái.
```const foo = null;
const bar = foo ?? 'default';
console.log(bar); // 'default'
```
2. Toán tử || (Logical OR Operator): Toán tử `||` trả về giá trị đầu tiên trong danh sách các toán hạng mà được coi là `true`. Nếu tất cả các toán hạng đều được coi là `false`, toán tử trả về toán hạng cuối cùng.
```
var value = null;
var defaultValue = 'Default Value';

var result = value || defaultValue;
console.log(result); // 'Default Value'

```
# Switch case trong Javascript
1. Cú pháp câu lệnh switch case
```
switch(x) {
  case 'value1':  // if (x === 'value1')
    ...
    [break]
  case 'value2':  // if (x === 'value2')
    ...
    [break]
  default:
    ...
    [break]
}
```
- Sau đây là ví dụ sử dụng lệnh switch case trong JavaScript:
```
const x = 2 + 3;
switch (x) {
  case 4:
    console.log("Less than");
    break;
  case 5:
    console.log("Equal");
    break;
  case 6:
    console.log("Greater than");
    break;
  default:
    console.log("Don't know the answer");
}
```
* Nếu không có từ khóa break thì sao?
Nếu không có từ khóa break thì toàn bộ khối lệnh phía sau case 5 được thực thi 

# Cấu trúc lặp trong Javascript
1. Vòng lặp while: Vòng lặp này thực hiện mã lặp lại một cách liên tục miễn là điều kiện xác định là true.
```while (condition) {
    // Thực hiện mã trong vòng lặp
}
```
2. Vòng lặp do...while: Vòng lặp này tương tự như vòng lặp while, nhưng nó sẽ thực hiện ít nhất một lần mã trong vòng lặp trước khi kiểm tra điều kiện.
```do {
    // Thực hiện mã trong vòng lặp
} while (condition);
```
3. Vòng lặp for: Vòng lặp này thực hiện mã lặp lại một số lần đã được xác định trước.

```
for (initialization; condition; increment) {
    // Thực hiện mã trong vòng lặp
}
```
4. Vòng lặp for...in: Vòng lặp này được sử dụng để liệt kê tất cả các thuộc tính có thể đếm được của một đối tượng.

```
for (variable in object) {
    // Thực hiện mã trong vòng lặp
}

```
5. Vòng lặp for...of: Vòng lặp này được sử dụng để lặp qua các đối tượng có thể lặp được như mảng, chuỗi, hoặc các cấu trúc dữ liệu tương tự.

```
for (variable of iterable) {
    // Thực hiện mã trong vòng lặp
}

```
# Tất tần tật về hàm trong Javascript
1. Hàm trong Javascript là gì?
- Hàm trong JavaScript là một chương trình con giúp thực thi một công việc cụ thể. Để định nghĩa hàm trong JavaScript, bạn sử dụng từ khoá function với cú pháp là:
```
function functionName([parameter1], [parameter2],...) {
  statement1;
  statement2;
  ...
}
```
2. Các lọai hàm trong javacript:
- Hàm thông thường (Regular Functions): Đây là loại hàm cơ bản được định nghĩa bằng từ khóa "function" và có tên cụ thể. Chúng có thể được gọi bằng cách sử dụng tên của hàm.
```
function regularFunction(parameters) {
    // Thân hàm
}
regularFunction(arguments);
```
- Hàm nặc danh (Anonymous Functions): Đây là loại hàm không có tên, thường được sử dụng như là các đối số của các hàm khác hoặc gán cho các biến. Chúng được khai báo mà không cần tên hàm.
```
var anonymousFunction = function(parameters) {
    // Thân hàm
};
anonymousFunction(arguments);

```
- Biểu thức hàm (Function Expressions): Đây là một biến thể của hàm nặc danh, trong đó hàm được gán cho một biến hoặc một biểu thức khác. Biểu thức hàm thường được sử dụng khi cần truyền hàm như một đối số.
``` 
var functionExpression = function(parameters) {
    // Thân hàm
};
functionExpression(arguments);

```
- Hàm mũi tên (Arrow Functions): Arrow functions là một cú pháp rút gọn để khai báo hàm, giúp viết mã ngắn gọn hơn và hỗ trợ ngữ cảnh "this" tốt hơn.
```
var arrowFunction = (parameters) => {
    // Thân hàm
};
arrowFunction(arguments);

```
# Tham trị và tham chiếu 
1. Tham trị (Pass by Value): Khi bạn truyền một giá trị kiểu dữ liệu nguyên thủy như số, chuỗi, hoặc boolean vào một hàm, một bản sao của giá trị đó sẽ được tạo ra và truyền vào hàm. Mọi thay đổi đối với bản sao này sẽ không ảnh hưởng đến giá trị gốc bên ngoài hàm.
```
let a = 5;

function changeValue(b) {
    b = b * 2;
    console.log(b); // Output: 10
}

changeValue(a);
console.log(a); // Output: 5

```
2. Tham chiếu (Pass by Reference): Khi bạn truyền một đối tượng hoặc mảng vào một hàm, một tham chiếu tới địa chỉ của đối tượng hoặc mảng đó sẽ được truyền vào hàm. Do đó, bất kỳ thay đổi nào được thực hiện trên đối tượng hoặc mảng trong hàm sẽ ảnh hưởng đến giá trị gốc bên ngoài hàm.
```
let obj = { value: 10 };

function changeObject(o) {
    o.value = 20;
    console.log(o.value); // Output: 20
}

changeObject(obj);
console.log(obj.value); // Output: 20

```

# Object 
1. So sánh 2 object bằng tham chiếu
- Đối với so sánh object bằng tham chiếu: hai object được gọi là bằng nhau khi và chỉ khi chúng cùng tham chiếu đến cùng một địa chỉ bộ nhớ. Hay nói ngắn gọn là chúng hoàn toàn giống nhau.
VD:
```
let x = {};
let y = x;
console.log(y == x); // true
console.log(y === x); // true
```
2. So sánh 2 object qua giá trị cách thủ công
- Đôi khi mình muốn so sánh thủ công từng giá trị ứng với từng thuộc tính của object. Và mình coi hai object bằng nhau khi chúng có cùng thuộc tính và cùng giá trị với từng thuộc tính.
Ví dụ có các object gồm thuộc tính sau:
```
let point1 = { x: 1, y: 2 };
let point2 = { x: 1, y: 2 };
let point3 = { x: 2, y: 3 };
```
- Làm sao để so sánh các point trên?
Đơn giản là mình sẽ truy cập giá trị của hai thuộc tính x và y trong từng object rồi so sánh chúng với nhau.
````
let point1 = { x: 1, y: 2 };
let point2 = { x: 1, y: 2 };
let point3 = { x: 2, y: 3 };
if (point2.x === point1.x && point2.y === point1.y) {
  console.log("point2 bằng point1");
} else {
  console.log("point2 khác point1");
}
if (point3.x === point1.x && point3.y === point1.y) {
  console.log("point3 bằng point1");
} else {
  console.log("point3 khác point1");
}
// point2 bằng point1
// point3 khác point1
``````
3. Copy Object trong Javascript
- Copy object sử dụng vòng lặp for...in
VD:
```
let p1 = { x: 1, y: 2 };
let p2 = {};
for (let key in p1) {
  p2[key] = p1[key];
}
console.log(p2.x); // 1
console.log(p2.y); // 2
p2.x = 5;
console.log(p2.x); // 5
console.log(p1.x); // 1
```
- Ngoài cách sử dụng vòng lặp for...in như trên, bạn có thể dùng hàm tương tự là Object.assign() với cú pháp:
```
Object.assign(dest, [src1, src2, src3...]);
```
3. Copy sâu 
- Để thực hiện copy sâu, bạn có thể dùng hàm JSON.stringify() để chuyển object về dạng JSON. Rồi sau đó, bạn dùng hàm JSON.parse() để tạo lại một object mới từ JSON.
```
let point1 = {
  x: 1,
  y: 2,
  metadata: {
    type: "point",
  },
};
// chuyển object về dạng JSON
let jsonPoint1 = JSON.stringify(point1);
console.log(jsonPoint1); // {"x":1,"y":2,"metadata":{"type":"point"}}
// parse JSON lại thành object mới
let point2 = JSON.parse(jsonPoint1);
console.log(point2.metadata.type); // point
point2.metadata.type = "CHANGED";
console.log(point2.metadata.type); // CHANGED
console.log(point1.metadata.type); // point
```

