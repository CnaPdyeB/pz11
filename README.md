![Uploading image.png…]()

Задание 1.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    for (int i = 1; i <= n; i++) {
        cout << i << " ";
    }
    return 0;
}

Задание 2.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    int sum = 0;
    for (int i = 1; i <= n; i++) {
        sum += i;
    }
    cout << sum;
    return 0;
}

Задание 3.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    // Ваш код:
    int num;
    int sum = 0;
    
    while (true) {
        cin >> num;
        if (num == 0) {
            break;
        }
        sum += num;
    }
    
    cout << sum;
    return 0;
}

Задание 4.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    for (int i = 1; i <= n; i++) {
        if (i % 2 == 0) {
            cout << i << " ";
        }
    }
    return 0;
}

Задание 5.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    long long factorial = 1;
    for (int i = 1; i <= n; i++) {
        factorial *= i;
    }
    cout << factorial;
    return 0;
}

Задание 6.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    
    // Если введён 0, то по условию игнорируем (выводим 0)
    if (n == 0) {
        cout << 0;
        return 0;
    }
    
    int count = 0;
    // Обрабатываем отрицательные числа (берём модуль)
    if (n < 0) {
        n = -n;
    }
    
    while (n > 0) {
        n /= 10;  // Удаляем последнюю цифру
        count++;   // Увеличиваем счётчик
    }
    
    cout << count;
    return 0;
}

Задание 7.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    
    // 1 не является простым числом
    if (n <= 1) {
        cout << "Не простое";
        return 0;
    }
    
    bool isPrime = true;
    
    // Проверяем делители от 2 до sqrt(n)
    for (int i = 2; i * i <= n; i++) {
        if (n % i == 0) {
            isPrime = false;
            break;
        }
    }
    
    if (isPrime) {
        cout << "Простое";
    } else {
        cout << "Не простое";
    }
    
    return 0;
}

Задание 8.
#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n;
    cin >> n;
    // Ваш код:
    
    int i = 1;
    while (i <= n) {
        int j = 1;
        while (j <= n) {
            cout << i * j << " ";
            j++;
        }
        cout << endl;
        i++;
    }
    
    return 0;
}
