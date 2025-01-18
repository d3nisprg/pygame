Pygame - графическая библиотека для создания ГРАФИЧЕСКОЙ части приложения на языке программирования Python.

Начнём с установки. Если у вас не установлена библиотека, можете написать в терминале
pip install pygame
Теперь после 
import pygame
можно начинать работу.

Для создания окна приложения нужно задать переменную окна. У меня sc
sc = pygame.display.set_mode()
Далее зададим переменную run. Если run = True, тогда приложение запущенно, иначе - нет.
run = True
while run:
Теперь перейдём к основной части. Весь функционал будем писать в WHILEе. Нужно добавить "функцию" закрытия приложения.
for event in pygame.event.get(): # перебор ивентов
    if event.type == pygame.QUIT: #если ивент - закрытие приложения
        run = False #выход
Теперь код:
import pygame

sc = pygame.display.set_mode()
run = True
while run:
  for event in pygame.event.get(): # перебор ивентов
      if event.type == pygame.QUIT: #если ивент - закрытие приложения
          run = False #выход
