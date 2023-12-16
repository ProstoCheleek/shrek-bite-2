import pygame


pygame.init()

screen_width = 1200
screen_height = 800

screen = pygame.display.set_mode((screen_width,screen_height))

font = pygame.font.SysFont("Arial",50)
font2 = pygame.font.SysFont("Arial",100)

shrek_bite = pygame.image.load("Шрек байт/Шрек байт.jpg")
shrek_bite = pygame.transform.scale(shrek_bite, (100,100))

hero = pygame.image.load("Шрек байт/герой.jpg")
hero = pygame.transform.scale(hero, (100,100))

fon = pygame.image.load(('Шрек байт/ФОН.jpg'))
fon = pygame.transform.scale(fon, (100, 100))



x,y =400, 100
x2,y2=400, 200
x3,y3 =400, 300
speed = 0.5
S, Z = 1, 1





while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            quit()


    screen.blit(fon, (500,1))

    screen.blit(hero, (500,1))

    screen.blit(shrek_bite, (S, Z))

    text = font.render('Начать играть', True, (0,220,0))
    screen.blit(text, (x,y))

    text2 = font.render('Настройки', True, (0, 220, 0))
    screen.blit(text2, (x2,y2))

    text3 = font.render('разрабы', True, (0, 220, 0))
    screen.blit(text3, (x3,y3))


    keys = pygame.key.get_pressed()
    if keys[pygame.K_d]:
        S += speed
    elif keys[pygame.K_a]:
        S -= speed

    elif keys[pygame.K_s]:
        Z += speed

    elif keys[pygame.K_w]:
        Z -= speed







    pygame.display.update()
