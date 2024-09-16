# REQUIREMENTS

Need Xcode 15 or playground 4 both Swift 5.9 or later.


# How To Run The App

To run the project, just open it with xcode or playground and App -> MyApp.swift. A preview of the app will appear, then you can build and run the app on the simulation.

# APP ICON
  
I draw an icon on my ipad with goodnotes 6 and Apple Pencil. I inspire myself from an image of African continent, then I used red color (to express blood, disease...) and black color (to express pain...), then, and I add some expressios or slogans on the image, and the result is inside the assets of the project. 
![Simulator Screenshot - iPhone 15 - 2024-09-16 at 06 01 29](https://github.com/user-attachments/assets/5c84246f-bc02-4023-a7fc-057f7a38ac1a)


# This game has 2 view:

The first is a play view where we can dive into different level and earn points. Each level is about one childabuse, and when you reached that level
a special card is unlocked for further information about abuse, and appears in the second view.

# Score
Each question we answer gives or removes points as
    - Each question correctly answered gives 10 points.
    - If we fail a question of one unique choice, we loose 5 points.
    - If a question has more than 2 answers: the game gives 5 points per correct answer and  for each false answer we loose 3 points. So if a question has 3 
      answers: if we find none of them we lose 5 points, if we find all of them we earn 10 points, and if we find 2 over 3 we earn 5*2-3=7.
         
The second view in a collection view where it's displaying all the locked and unlocked card for all levels.
Each card displays some relevant informations: the name of the abuse, his colorImpact, his gravity rank, and the rate presence or scope.

# Abuse
The game recensed 12 major child abuse present in Africa among:

1)  Unsheltered Children
2)  Hungry
3)  Early Sex Initiation of Girls
4)  Missing Medical Care
5)  Kidnapping
6)  Girls Forced Marriage
7)  Children Labor
8)  Child Soldiers
9)  Unschooled Children
10) Girls Genitaliq mutilation
11) Child Sacrifices
12) Children Beaten

# Gravity
- Gravity is a number between 1 to 12 which gives an idea of the harmful impacts the abuse brings on the life of concerned children. It provides a correlated information with ColorImpact. This number is apprioximately ranging abuses between the overall listed in this game. So gravity 1/12 is the worst one and so on. In this ranking, the worst ranked ( with lower rank ) abuses are those with direct impacts on children's life (cause death, deseases...). Also we take in cosideration the rate presence in the continent (the number of cildren victims amoung african children).

# ColorImpact
- cardColorImpac takes one or more color among these 5 colors:

    -black = death
    -green = child labour / sufference / slaving / exploitation
    -red = disease/abuse (like rape or sexual abuse)
    -blue = physical and mental dammages
    -indigo = attemps to personal development (like forced marriage)
    
    This color represent the dominant impact of the corresponding childabuse.
    When a card has many color we find the mix of these colors: example blue + red =  purple.


# Infos
Each card contains some further infos about abuse and links to websites used to fetch infos to build questions.

# Scope

It's simply the percentage of cildren victim of the abuse among the overall African children. It's an approximetion. Africa has around 400-500 Million children


# Music

The project includes some sound effects. These sounds are free licence sounds donwload on https://www.freesoundslibrary.com

"Free Sounds Library"


Free Sound Effects Site.


Licence: License: Attribution 4.0 International (CC BY 4.0). You are allowed to use sound effects free of charge and royalty free in your multimedia projects for commercial or non-commercial purposes.


http://www.freesoundslibrary.com


# Code and SwiftView/file

CardCollectionView: conatains all structs for flipped and unflipped cards

CardData: contains all data of the cards = scope, gravity, color impact, abuse name

PlayerData:  contains a class names player with all infos of a player(name, score, last level, last question Id, higher level reached...) and a class to play sound in a game and an enumeration of all available sounds.

QuestionData: contains all the questions and answer, but also a list of expression to encourage the user to play

QuestionView: contains all the structs of the form of the game, with check button , validate button, the menu to choose the level...

Ressours: contains two folders of the game's sounds.
