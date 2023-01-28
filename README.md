# Accept-Functions-as-arguments

function transform(fn, arr) {
 let result = [];
 for (let el of arr) {
 result.push(fn(el)); // We push the result of the transformed item to result
 }
 return result;
}
console.log(transform(x => x * 2, [1,2,3,4])); // [2, 4, 6, 8]
