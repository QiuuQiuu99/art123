import (requests)

url = "https://www.example.com"
response = requests.get(url)

if response.status_code == 200:
    print("Запрос успешно выполнен")
    print(f"Код состояния: {response.status_code}")
    print(f"HTML-код страницы:\n{response.text}")
else:
    print("Что-то пошло не так")
    print(f"Код состояния: {response.status_code}")
