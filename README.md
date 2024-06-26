function greatestCommonDivisor(x, y) {
    while (y !== 0) {
        let temp = y;
        y = x % y;
        x = temp;
    }
    return x;
}

// Пример использования
let num1 = 48;
let num2 = 18;
let result = greatestCommonDivisor(num1, num2);
console.log("Наибольший общий делитель:", result);
