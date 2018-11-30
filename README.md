# fa18-202-pheonix

Phoenix team has developed a single player game called "The walking Dead".

## Team members:

Kriti Jar

Ruchika Hazariwal

Harsh Agarwal

Hemaprasanthi Mutyala

## Design Patterns

### State Design Pattern: For game Levels (Kriti Jar)

LevelOneState: Initial level of game. It includes 5 zombies.

LevelTwoState: The number of zombies are 8 in level two. 

LevelThreeState: The number of zombies are 10. Once the zombies are killed Final banner is shown.

### Observer Design Pattern (Kriti Jar)

Subject: Human and Bullet

Observers: ItemCollectionObserver and SoundObserver

Observer pattern keep tracks of all the items which are intersected by human or bullet and notifies the observers.
Ex. When human collects kit, ItemCollectionObserver is notifies that updates the message to 'Kit Available'.

If human, collects the sword, soundObserver is notified that plays the sound in background.

### Facade Pattern: Simplifying ItemCollectionObserver (Ruchika Hazariwal)

The Facade pattern was implemented to simplify the complex ItemCollectionObserver functionalities.
It helped in distributing the task  and providing the simplified interface.

Overall ItemCollectionObserver was simplified to KitFacade, SwordFacade, HumanFacade, ZombieFacade, ZombieBulletFacade.

### State Design Pattern : Human State (Ruchika Hazariwal)
iHumanState

HumanAliveState: Human is alive and if collides zombie then set state to humanDeadState 

HumanDeadState: If human dies, state changes to HumanDeadState.

### State Design Pattern: Sword State (Harsh Agarwal)
iSwordState

NoSwordState: Human doesn't have any sword parts.

HalfSwordState: Human has one part of sword and same is updated to message

FullSwordState: Human has both parts of sword and can kill one zombie.

### Factory Pattern: Creating actors (Harsh Agarwal)

KitFactory: To create kit
ZombieFactory: To create zombie
FoodFactory: To create Food
GunFactory: To create gun
SwordFactory: To create parts of sword

### Strategy Pattern: Human and Zombie movement (Hemaprasanthi Mutyala)













