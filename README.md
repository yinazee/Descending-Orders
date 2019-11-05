# Descending-Orders
Code Challenge

Your task is to make a function that can take any non-negative integer as a argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

Examples:
Input: 21445 Output: 54421

Input: 145263 Output: 654321

Input: 1254859723 Output: 9875543221

Solution:

function descendingOrder(n){
  return parseInt(String(n).split('').sort().reverse().join(''))
}

My Solution:

function descendingOrder(n){

  let num = n.toString();

  let str = num.split("");

  let integers = str.map(can => parseInt(can))

  let sorted = integers.sort(function(a, b){return b-a})

  return parseInt(sorted.join(""))

}
