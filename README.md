function isEnoughCapacity(products, containerSize){
    let totalItems = 0;
    for (let product in products) {
        totalItems += products[product];
    }
    return totalItems <= containerSize;
};


Напиши функцію calcAverageCalories(days), яка повертає середньодобове значення кількості калорій, які спортсмен споживав протягом тижня. Функція очікує один параметр: days — масив об’єктів. Кожен об’єкт описує день тижня та кількість калорій calories, спожитих спортсменом, у цей день. Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її викликів.

function calcAverageCalories(days) {
    let totalCalories = 0;
    for (let i = 0; i < days.length; i++) {
        totalCalories += days[i].calories;
    }

    return totalCalories / days.length;
}
