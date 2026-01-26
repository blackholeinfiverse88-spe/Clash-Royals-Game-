# Demo Scope Declaration


### 1. Card System (Data-Driven)

* Cards are driven by **ScriptableObjects (`UnitData`)**
* Each card contains:

  * Unit Name
  * Cost
  * Icon (Card Image)
  * Description
  * Unit Prefab reference

### 2. Deck Builder

* Players can:

  * View all available cards
  * Select and deselect cards
  * Build a deck with a **fixed maximum size**
* Visual feedback updates in real time

### 3. Card UI

* Card UI is generated at runtime using a reusable **Card Prefab**
* Card visuals (name, cost, icon) are populated dynamically via code
* No card images or data are hardcoded into prefabs

### 4. Scene Flow

* Deck selection scene
* Transition to battle scene once deck is complete

## Design Philosophy

* **Separation of concerns**

  * Data (`UnitData`) is separate from UI (`CardUI`)
  * UI does not store gameplay data

* **Scalable architecture**

  * New cards can be added without modifying code
  * Card UI prefab is reusable





